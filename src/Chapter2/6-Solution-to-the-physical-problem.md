# 最速曲线问题的解答

回到最开始的问题，我们已知
$$
T=\int_0^{X} \frac{\sqrt{1+y^{\prime 2}}}{\sqrt{2gy}} dx
$$
注意到$x$并不显含于$F$，因此可以用前面的欧拉方程的另一种形式
$$
F-y^{{}\prime}\cdot \frac{\partial F}{\partial y^{\prime}}=C
$$
有
$$
\frac{\partial F}{\partial y^{\prime}}=(2gy)^{-\frac{1}{2}}(1+y^{\prime2})^{-\frac{1}{2}}y^{\prime}
$$
代入欧拉方程
$$
\frac{\sqrt{1+y^{\prime2}}}{\sqrt{2gy}}-\frac{y^{\prime2}}{\sqrt{2gy}\sqrt{1+y^{\prime2}}}=C
$$
合并移项得
$$
(1+(\frac{dy}{dx})^2)y=\frac{1}{2gC^2}
$$
注意$\frac{1}{2gC^2}$是一个常数，我们令其为$k$
$$
(\frac{dy}{dx})^2=\frac{k-y}{y}
$$
所以
$$
\sqrt{\frac{y}{k-y}}dy=dx
$$
注意到
$$
\sqrt{\frac{y}{k-y}} = \sqrt{\frac{y/k}{1-\frac{y}{k}}}
$$
令$y/k=w$那么
$$
\sqrt{\frac{y}{k-y}} = \sqrt{\frac{w}{1-w}}
$$
此时可以令$w=\frac{1}{2}(1-\cos \theta)$，因此
$$
\sqrt{\frac{y}{k-y}} =\sqrt{\frac{\frac{1}{2}(1-\cos \theta)}{\frac{1}{2} (1+\cos \theta)}}=\frac{1-\cos \theta}{\sin \theta}
$$
所以可以进行换元，令$y=\frac{k}{2}(1-\cos\theta)\quad dy=\frac{k}{2}\sin\theta d\theta$

所以
$$
\sqrt{\frac{y}{k-y}}dy=\sqrt{\frac{1-\cos\theta}{1+\cos\theta}}\sqrt{\frac{1-\cos\theta}{1-\cos\theta}}\cdot\frac{k}{2}\sin\theta d\theta =dx
$$
化简得
$$
\frac{k}{2}(1-\cos\theta)d\theta=dx
$$
对两边积分即可解出方程，得
$$
x=\frac{k}{2}(\theta-\sin \theta)+C^\prime
$$
又已知$y_0=x_0=0$（过原点），因此可得最终的参数方程解
$$
\left\{\begin{aligned}y&=\frac{k}{2}(1-\cos\theta)\\x&=\frac{k}{2}(\theta-\sin\theta)\end{aligned}\right.
$$