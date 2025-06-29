# The Solow model



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
> 有了上面的推导，实际上某一时刻的人口是解微分方程得出来的，即
> $$
> \int \frac{\partial \ln L}{\partial t} dt = \int n dt
> $$
> 此后的一些模型也会利用这一公式。



## The (neoclassical) production function

忽略技术进步，即假设$F(\cdot)$与$t$无关，此时 $Y=F(K,L)$。若一个生产函数的具体形式满足以下三个假设，则可被称之为新古典生产函数：



### 假设一

对于所有 $K > 0 $和$ L > 0$，$F(⋅)$ 输出的边际产量为正且递减，即：
$$
\frac{\partial F}{\partial K} >0\quad \frac{\partial F}{\partial L} >0 \quad \text{（边际产量为正）}\quad
	\frac{\partial^{2} F}{\partial K^{2}} <0\quad \frac{\partial^{2} F}{\partial L^2} <0 \quad \text{（边际产量递减）}
$$


### 假设二

规模报酬不变（Constant returns to scale，CRS）
$$
\text{For all } \lambda >0, F(\lambda K, \lambda L)= \lambda F(K,L)
$$


### 假设三（稻田条件）

资本（或劳动力）投入趋于 0 时，其边际产量趋近于无穷大；而当资本（或劳动力）投入趋于无穷大时，其边际产量趋近于 0。
$$
	\lim_{K\rightarrow 0} \frac{\partial F}{\partial K} =\lim_{L\rightarrow 0} \frac{\partial F}{\partial L} =\infty \quad \lim_{K\rightarrow \infty} \frac{\partial F}{\partial K} =\lim_{L\rightarrow \infty} \frac{\partial F}{\partial L} =0
$$


科布·道格拉斯函数（下简称 CD 函数）满足上述三个条件，就是一个新古典生产函数，其形式为:
$$
Y=AK^{\alpha}L^{1-\alpha}
$$
$A>0$ 为技术水平，人均生产函数为 $Ak^\alpha$



