# 外生技术增长的 Solow 模型



现允许要素生产率随时间变化，在 CD 函数中，这意味着 $A$ 随时间增加。设$\frac{\dot{A}}{A}=a>0$，在还未达到 BGP 时：
$$
\frac{\dot{y}}{y}=\frac{\dot{y}}{y} + \alpha \cdot \frac{\dot{k}}{k} = a + \alpha \cdot \gamma_k
$$

在 BGP 时，$k$为常数，此时
$$
\frac{\dot{y}}{y}=a
$$

**结论**：从长远来看，技术进步是人均收入增长的唯一来源。



先将技术进步融入劳工：$L$不仅仅为劳动人口，而是人力资本，定义：
$$
E_t=L_t \cdot e^{\lambda t}=L_0\cdot e^{(\lambda+n)t}
$$

此时生产函数为 $Y=F(K_t, E_t)$。从人均效率角度看，可以定义$k=\frac{K}{E}$，那么$\dot{k} = \frac{\dot{K}E-K\dot{E}}{E^2}$，此时
$$
\begin{aligned}\frac{\dot{k}}{k}&=\frac{\dot{K} E-K\dot{E}}{E^{2}} \cdot \frac{E}{K}\\ &=\frac{\dot{K} E-K\dot{E}}{KE} =\frac{\dot{K}}{K} -\frac{\dot{E}}{E}\end{aligned}
$$

在 (1.7) 式已知$\gamma_k = \frac{\dot{k}}{k} = \frac{sf(k)}{k}-(n+\delta)$，所以代入可得
$$
\frac{\dot{k}}{k}=\frac{sf(k)}{k}-\delta-n-\lambda
$$

两侧乘以$k$得
$$
\dot{k}=sf(k)-(\delta+n+\lambda)k
$$

当$\dot{k}=0$时，$\frac{sf(k)}{k}=(\delta+n+\lambda)$

$\dot{k}=0$时，处于BGP，因此
$$
\frac{\dot{K}}{K}=\frac{\dot{E}}{E}=n+\lambda=\frac{\dot{Y}}{Y}
$$

长期来看
$$
    \frac{\dot{\left(\frac{Y}{L}\right)}}{\frac{Y}{L}}=\frac{\dot{Y}}{Y}-\frac{\dot{L}}{L}=\lambda
$$
（因为$\frac{\dot{Y}}{Y}=\lambda + n, \frac{\dot{L}}{L}=n$）