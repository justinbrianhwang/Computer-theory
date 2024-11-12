| $ x(t) $                           | $ X(\omega) $                                             |
|--------------------------------------|-------------------------------------------------------------|
| $1$                                  | $2\pi \delta(\omega)$                                       |
| $u(t)$                               | $\pi \delta(\omega) + \frac{1}{j\omega}$                    |
| $\delta(t)$                          | $1$                                                         |
| $\delta(t - t_0)$                    | $e^{-j\omega t_0}$                                          |
| $\text{rect}(t/\tau)$                | $\tau \text{sinc}\left(\frac{\omega \tau}{2}\right)$        |
| $\frac{\sin(\omega_0 t)}{\pi t}$     | $\text{rect}\left(\frac{\omega}{2\omega_0}\right)$          |
| $\text{sgn}(t)$                      | $\frac{2}{j\omega}$                                         |
| $e^{j\omega_0 t}$                    | $2\pi \delta(\omega - \omega_0)$                            |
| $\sum_{n=-\infty}^{\infty} \delta(t - nT)$ | $\frac{2\pi}{T} \sum_{n=-\infty}^{\infty} \delta\left(\omega - \frac{2\pi n}{T}\right)$ |
| $\cos(\omega_0 t)$                   | $\pi [\delta(\omega - \omega_0) + \delta(\omega + \omega_0)]$ |
| $\sin(\omega_0 t)$                   | $\frac{\pi}{j} [\delta(\omega - \omega_0) - \delta(\omega + \omega_0)]$ |
| $(\cos(\omega_0 t)) u(t)$            | $\frac{\pi}{2} [\delta(\omega - \omega_0) + \delta(\omega + \omega_0)] + \frac{j\omega}{\omega_0^2 - \omega^2}$ |
| $(\sin(\omega_0 t)) u(t)$            | $\frac{\pi}{2} [\delta(\omega - \omega_0) - \delta(\omega + \omega_0)] + \frac{\omega_0}{\omega_0^2 - \omega^2}$ |
| $\cos(\omega_0 t) \text{rect}(t/\tau)$ | $\tau \text{sinc}\left(\frac{\omega - \omega_0}{2\pi}\right) + \tau \text{sinc}\left(\frac{\omega + \omega_0}{2\pi}\right)$ |
| $e^{-a t} u(t), \ \text{Re}(a) > 0$  | $\frac{1}{a + j\omega}$                                      |
| $t e^{-a t} u(t), \ \text{Re}(a) > 0$ | $\frac{1}{(a + j\omega)^2}$                                  |
| $\frac{t^{n-1}}{(n-1)!} e^{-a t} u(t), \ \text{Re}(a) > 0$ | $\frac{1}{(a + j\omega)^n}$                                |
| $|t| e^{-a |t|}, \ a > 0$            | $\frac{2a}{a^2 + \omega^2}$                                  |
| $|t| e^{-a |t|}, \ \text{Re}(a) > 0$ | $\frac{4a j\omega}{a^2 + \omega^2}$                          |
| $\frac{1}{a^2 + t^2}, \ \text{Re}(a) > 0$ | $\frac{\pi}{a} e^{-a|\omega|}$                            |
| $\frac{t}{a^2 + t^2}, \ \text{Re}(a) > 0$ | $-\frac{j\pi\omega e^{-a|\omega|}}{2a}$                     |
| $e^{-a^2 t^2}$                       | $\sqrt{\frac{\pi}{a}} e^{-\frac{\omega^2}{4a}}$             |
| $\Delta(t/\tau)$                     | $\tau \text{sinc}\left(\frac{\omega \tau}{2\pi}\right)$     |
| $\sum_{n=-\infty}^{\infty} \delta(t - nT)$ | $\frac{2\pi}{T} \sum_{n=-\infty}^{\infty} \delta\left(\omega - \frac{2\pi n}{T}\right)$ |
