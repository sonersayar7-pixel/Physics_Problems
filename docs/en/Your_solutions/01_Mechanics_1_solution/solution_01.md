section{11.1: Projectile Motion Analysis}

subsection*{1. Initial Conditions}
A projectile is launched from ground level with initial velocity $v_0 = 100 \text{ m/s}$ at an angle $\theta = 37^\circ$. We first decompose the velocity into orthogonal components:
begin{itemize}
    \item $v_{0x} = v_0 \cos(37^\circ) = 100 \times 0.8 = 80 \text{ m/s}$
    \item $v_{0y} = v_0 \sin(37^\circ) = 100 \times 0.6 = 60 \text{ m/s}$
end{itemize}

subsection*{2. Differential Equations of Motion}
Using Newton's Second Law ($\vec{F} = m\vec{a}$), and assuming gravity $g$ is the only force:

subsubsection*{Horizontal Direction ($x$)}
Since there is no air resistance, $F_x = 0$:
$$m \frac{d^2x}{dt^2} = 0 \implies \frac{d^2x}{dt^2} = 0$$
Integrating once gives constant horizontal velocity: $v_x(t) = v_{0x}$.

subsubsection*{Vertical Direction ($y$)}
The force of gravity acts in the negative $y$ direction, $F_y = -mg$:
$$m \frac{d^2y}{dt^2} = -mg \implies \frac{d^2y}{dt^2} = -g$$
Integrating once gives vertical velocity: $v_y(t) = v_{0y} - gt$.



subsection*{3. Time of Flight ($t_f$)}
The projectile returns to the ground when vertical displacement $y(t) = 0$. Using $y(t) = v_{0y}t - \frac{1}{2}gt^2$:
$$0 = t(v_{0y} - \frac{1}{2}gt) \implies t_f = \frac{2v_{0y}}{g}$$
$$t_f = \frac{2(60)}{9.8} \approx 12.24 \text{ s}$$

subsection {4. Maximum Height ($H$)}
Maximum height occurs when the vertical velocity $v_y = 0$: