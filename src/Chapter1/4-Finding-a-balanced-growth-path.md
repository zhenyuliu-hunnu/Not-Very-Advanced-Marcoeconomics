# 平衡增长路径

平衡增长路径（balanced growth path，以下简称 BGP）指的是各种量以恒定速率增长的情况。

> [!IMPORTANT]
>
> BGP常被称为「稳态」，这一术语借自经典物理学。我们注意到，「稳态」的表述往往让学生误以为变量完全停止增长。实际上其正确定义是指增长率保持恒定，正如我们将要看到的，只有在特定情况下对某些变量而言，这种恒定增长率才会恰好为零。


在 Solow 模型中，BGP 对应为 $\dot{k}=0$，对应值为 $k^{\ast}$，满足：
$$
sf(k^{\ast})=(n+\delta)k^{\ast}
$$
在BGP中，资本劳动比$k$保持恒定，人均产出$k$和人均消费$c$稳定在$y^{\ast}=f(k^{\ast})$和$c^{\ast}=(1-s)f(k^{\ast})$的水平。



> [!Note]
>
> **所以在 Solow 模型中，人均量不增长了吗？**
>
> **不对。** 人均量虽然不增长，但总量$K,Y,C$在 BGP 中以人口增长率$n$的速度增长，此外，技术进步、储蓄率$s$、折旧率$\delta$都会对 BGP时的人均水平产生影响。


现代入CD函数$f(k)=Ak^{\alpha}$，可得BGP中
$$
k^{\ast}=\left(\frac{sA}{n+\delta}\right)^{\frac{1}{1-\alpha}}=A^{\frac{1}{1-\alpha}}\left(\frac{s}{n+\delta}\right)^{\frac{\alpha}{1-\alpha}}\quad (0<\alpha<1)
$$
这里可以看到，$k^{\ast}$随$s$和$A$的上升而上升，随$n$和$\delta$的下降而下降。