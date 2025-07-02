# Solow 模型



生产函数 $Y=F(K,L,t)$

其中 $Y$ 为产出，可以被消费（$C$）或投资（$I$）以创造新的实物资本单位。

$s$ 为被保存的产出比例，$1-s$为被消费的产出比例，$0 \leqslant s \leqslant 1$

$\delta$为折旧率，以此可计算某一时间点实物资本存量的增量：

$$
\dot{K} =I-\delta \cdot K=s\cdot F\left( K,L,t \right) -\delta \cdot K
$$
其中$\dot{K}$表示对时间的微分。

> [!Important]
>
> 一个变量对时间的微分表达为：$\dot{K}=\frac{\partial K}{\partial t}$，之所以可以微分是因为$K$也是关于时间$t$的函数而不是一个变量，这是本书的一处变动，目的是减少大量的括号表达。

假设人口就是劳动力$L$，它以恒定的外生速率$n=\frac{\dot{L}}{L}\geq0$增长，若 $t=0$ 时人口归化为1，那么$t$时的人口$L_t=e^{nt}$

> [!Important]
>
> 在宏观经济学中，一个变量的增长率常用这个变量对时间的微分除以这个变量本身。原因在于首先需要将变量做指数平滑，并对其自身求导，即$\frac{\partial \ln L}{\partial L}=\frac{1}{L}$，然后需要乘以这个变量对时间的微分，即$\dot{L}=\frac{\partial L}{\partial t}$，两式相乘可以发现$\frac{\dot{L}}{L}=\frac{\partial \ln L}{\partial t}$



> [!Tip]
>
> 有了上面的推导，实际上某一时刻的人口是两边积分得出来的，即
> $$
> \int \frac{\partial \ln L}{\partial t} dt = \int n dt
> $$
> 此后的一些模型也会利用这一公式。
