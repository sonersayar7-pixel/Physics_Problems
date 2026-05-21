<!DOCTYPE html>
<html>
<head>
    <title>Simple Pendulum Simulator</title>
    <style>
        body { font-family: Arial; text-align: center; margin-top: 50px; }
        canvas { background: #eef; border: 1px solid #ccc; }
        button { padding: 10px 20px; font-size: 16px; margin-top: 20px; cursor: pointer; }
        #stopwatch { font-size: 24px; margin-top: 10px; font-weight: bold; color: red; }
    </style>
</head>
<body>
    <h2>Simple Pendulum</h2>
    <p>Length (L) = 1.0 m (Exact) | Initial Angle = Small</p>
    <canvas id="pendulumCanvas" width="400" height="300"></canvas><br>
    <div id="stopwatch">Stopwatch: 0.00 s</div>
    <button id="toggleBtn" onclick="toggleSim()">Start</button>
    <button onclick="resetSim()">Reset</button>

    <script>
        const canvas = document.getElementById('pendulumCanvas');
        const ctx = canvas.getContext('2d');
        let t = 0, isRunning = false, interval;
        const L = 200, g = 9.81, omega = Math.sqrt(g / 1.0); 
        const theta_max = 0.2; // Small angle approximation

        function drawPendulum(theta) {
            ctx.clearRect(0, 0, canvas.width, canvas.height);
            let pivotX = 200, pivotY = 20;
            let bobX = pivotX + L * Math.sin(theta);
            let bobY = pivotY + L * Math.cos(theta);
            
            // Draw ceiling
            ctx.fillStyle = '#333'; ctx.fillRect(150, 0, 100, 20);
            // Draw string
            ctx.beginPath(); ctx.moveTo(pivotX, pivotY); ctx.lineTo(bobX, bobY); ctx.stroke();
            // Draw bob
            ctx.beginPath(); ctx.arc(bobX, bobY, 15, 0, 2*Math.PI);
            ctx.fillStyle = '#e74c3c'; ctx.fill(); ctx.stroke();
        }

        function update() {
            t += 0.02;
            let theta = theta_max * Math.cos(omega * t);
            drawPendulum(theta);
            document.getElementById('stopwatch').innerText = `Stopwatch: ${t.toFixed(2)} s`;
        }

        function toggleSim() {
            if(isRunning) { clearInterval(interval); isRunning=false; document.getElementById('toggleBtn').innerText = "Start"; }
            else { interval = setInterval(update, 20); isRunning=true; document.getElementById('toggleBtn').innerText = "Stop"; }
        }
        
        function resetSim() {
            clearInterval(interval); isRunning = false; t = 0;
            document.getElementById('toggleBtn').innerText = "Start";
            document.getElementById('stopwatch').innerText = `Stopwatch: 0.00 s`;
            drawPendulum(theta_max);
        }
        drawPendulum(theta_max);
    </script>
</body>
</html>