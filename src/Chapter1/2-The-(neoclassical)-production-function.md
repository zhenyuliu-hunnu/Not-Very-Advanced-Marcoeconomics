# （新古典）生产函数

忽略技术进步，即假设$F(\cdot)$与$t$无关，此时 $Y=F(K,L)$。若一个生产函数的具体形式满足以下三个假设，则可被称之为新古典生产函数：



## 假设一

对于所有 $K > 0 $和$ L > 0$，$F(⋅)$ 输出的边际产量为正且递减，即：
$$
\frac{\partial F}{\partial K} >0\quad \frac{\partial F}{\partial L} >0 \quad \text{（边际产量为正）}\quad
	\frac{\partial^{2} F}{\partial K^{2}} <0\quad \frac{\partial^{2} F}{\partial L^2} <0 \quad \text{（边际产量递减）}
$$



## 假设二

规模报酬不变（Constant returns to scale，CRS）
$$
\text{For all } \lambda >0, F(\lambda K, \lambda L)= \lambda F(K,L)
$$

假设二的存在，可以使得生产函数被表示为
$$
Y=F(K,L)=L \cdot F(\frac{K}{L}, 1)=L\cdot f(k)
$$
其中$k\equiv \frac{K}{L}$，即资本/劳动比率。此时生产函数可被写为$L \cdot F(k, 1)$即$L\cdot f(k)$，即可定义生产函数的人均形式$y=f(k)$。



## 假设三（稻田条件）

资本（或劳动力）投入趋于 0 时，其边际产量趋近于无穷大；而当资本（或劳动力）投入趋于无穷大时，其边际产量趋近于 0。
$$
	\lim_{K\rightarrow 0} \frac{\partial F}{\partial K} =\lim_{L\rightarrow 0} \frac{\partial F}{\partial L} =\infty \quad \lim_{K\rightarrow \infty} \frac{\partial F}{\partial K} =\lim_{L\rightarrow \infty} \frac{\partial F}{\partial L} =0
$$


科布·道格拉斯函数（下简称 CD 函数）满足上述三个条件，就是一个新古典生产函数，其形式为:
$$
Y=AK^{\alpha}L^{1-\alpha}
$$
$A>0$ 为技术水平，人均生产函数为 $Ak^\alpha$