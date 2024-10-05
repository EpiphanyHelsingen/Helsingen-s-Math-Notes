**级数 $\sum\limits_{k=1}^{\infty} \frac{\sin kx}{k}$ 的求法**
$$
\begin{align}
\sum\limits_{k=1}^{\infty} \frac{\sin kx}{k}
&=\sum\limits_{k=1}^{\infty}\int_{0}^{x}\cos kt  \, dt \\
&=\int _{0}^{x}\sum\limits_{k=1}^{\infty}\cos kt \, dt  \\
&=\lim\limits_{ n \to \infty }\int _{o}^{x}\sum\limits_{k=1}^{n}\cos kt \, dt \\
&=\lim\limits_{ n \to \infty }\int _{o}^{x} \frac{\sin \frac{2n+1}{2}t}{2\sin \frac{t}{2}} \,dt -\frac{x}{2}  
\end{align}
$$
其中
$$
\int_{o}^{x}\frac{\sin \frac{2 n+1}{2}t}{2\sin \frac{t}{2}} \, dt -\frac{x}{2}
=-\frac{x}{2}+\int _{0}^{x}\left( \frac{1}{2\sin \frac{t}{2}}-\frac{1}{t} \right)\sin(2n+1) \frac{t}{2} \, dt+\int _{0}^{x} \frac{\sin(2n+1) \frac{t}{2}}{t} \, dt  
$$
下面运用[[14.2.2. Riemann 第一引理]]

易知 $\displaystyle \frac{1}{t}$ 在 $\displaystyle [0,x]$ 上不绝对可积,下证 $\displaystyle \frac{1}{2\sin \frac{t}{2}}-\frac{1}{t}$ 在 $\displaystyle [0,x]$ 上绝对可积.

$$
\lim\limits_{ t \to 0 }\frac{t-2\sin \frac{t}{2}}{2t\sin \frac{t}{2}}=\lim\limits_{ t \to {0} } \frac{\frac{1}{2}\sin \frac{t}{2}}{2\cos \frac{t}{2}-\frac{1}{2}t\sin \frac{t}{2}}=0   
$$

易知 $\displaystyle \nexists\lim\limits_{ t \to {2k\pi} } (\frac{1}{2\sin \frac{t}{2}}-\frac{1}{t}),k=1,2,\dots$ 故 $\displaystyle \frac{1}{2\sin \frac{t}{2}}-\frac{1}{t}$ 在 $\displaystyle [0,x]，x<2k\pi$ 上绝对可积.

故
$$
\lim\limits_{ n \to {\infty} } \int _{0}^{x}\left( \frac{1}{2\sin \frac{t}{2}}-\frac{1}{t} \right)\sin(2n+1) \frac{t}{2} \, dt=0
$$
下求 $\lim\limits_{ n \to {\infty} } \int _{0}^{x} \frac{\sin(2n+1) \frac{t}{2}}{t} \, dt$, 令 $\displaystyle u=\frac{2n+1}{2}t,$ 则

$$
\lim\limits_{ n \to {\infty} } \int _{0}^{x} \frac{\sin(2n+1) \frac{t}{2}}{t} \, dt=\lim\limits_{ n \to {\infty} } \int _{0}^{\frac{2n+1}{2}x} \frac{\sin u}{u} \,du=\int _{0}^{\infty} \frac{\sin u}{u}\, du=\frac{\pi}{2} 
$$

故
$$
\sum\limits_{k=1}^{\infty} \frac{\sin kx}{k}=\frac{\pi-x}{2}
$$
