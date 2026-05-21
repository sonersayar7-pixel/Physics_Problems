<!DOCTYPE html>
<html>
<head>
    <title>Mass-Spring Simulator</title>
    <style>
        body { font-family: Arial; text-align: center; margin-top: 50px; }
        canvas { background: #f4f4f4; border: 1px solid #ccc; }
        button { padding: 10px 20px; font-size: 16px; margin-top: 20px; cursor: pointer; }
        #timer { font-size: 24px; margin-top: 10px; font-weight: bold; }
    </style>
</head>
<body>
    <h2>Mass-Spring System</h2>
    <p>Mass (m) = 1.0 kg (Exact) | Spring Constant (k) = 39.47 N/m</p>
    <canvas id="simCanvas" width="300" height="400"></canvas><br>
    <div id="timer">Time: 0.00 s</div>
    <button onclick="startSim()">Start / Reset</button>

    <script>
        const canvas = document.getElementById('simCanvas');
        const ctx = canvas.getContext('2d');
        let t = 0, isRunning = false, interval;
        const mass = 1.0, k = 39.47; 
        const omega = Math.sqrt(k / mass); // Angular frequency

        function drawSystem(yOffset) {
            ctx.clearRect(0, 0, canvas.width, canvas.height);
            // Draw ceiling
            ctx.fillStyle = '#666'; ctx.fillRect(100, 0, 100, 20);
            // Draw spring
            ctx.beginPath(); ctx.moveTo(150, 20);
            for(let i=0; i<15; i++) {
                ctx.lineTo(i%2===0 ? 140 : 160, 20 + i*((150+yOffset)/15));
            }
            ctx.lineTo(150, 170 + yOffset); ctx.stroke();
            // Draw mass
            ctx.fillStyle = '#3498db';
            ctx.fillRect(125, 170 + yOffset, 50, 50);
        }

        function update() {
            t += 0.02;
            let yOffset = 100 * Math.cos(omega * t); // Amplitude = 100px
            drawSystem(yOffset);
            document.getElementById('timer').innerText = `Time: ${t.toFixed(2)} s`;
        }

        function startSim() {
            if (isRunning) { clearInterval(interval); t=0; isRunning=false; drawSystem(100); }
            else { interval = setInterval(update, 20); isRunning=true; }
        }
        drawSystem(100); // Initial state
    </script>
</body>
</html>