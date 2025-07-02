# 另一种形式的欧拉方程

现在对$F(x,y,y')$做$x$的全微分：
$$
\frac{\partial F}{\partial x} =\frac{\partial F}{\partial x} \cdot \frac{\partial x}{\partial x} +\frac{\partial F}{\partial y} \cdot \frac{\partial y}{\partial x} +\frac{\partial F}{\partial y'} \cdot \frac{\partial y'}{\partial x} = \frac{\partial F}{\partial x}  + \frac{\partial F}{\partial y} \cdot y^\prime +\frac{\partial F}{\partial y'} \cdot y^{\prime \prime} $$

考虑这样一个函数的微分
$$
\frac{\partial}{\partial x} \left( y^{{}\prime}\cdot \frac{\partial F}{\partial y^{\prime}} \right) =y^{\prime \prime}\frac{\partial F}{\partial y^{\prime}} +y^{\prime}\cdot \frac{\partial}{\partial x} (\frac{\partial F}{\partial y^{\prime}} )
$$
由全微分可推知
$$
\frac{\partial F}{\partial y'} \cdot y^{\prime \prime} = \frac{\partial F}{\partial x} - \frac{\partial F}{\partial x}- \frac{\partial F}{\partial y} \cdot y^\prime 
$$
将其代入得
$$
\frac{\partial}{\partial x} \left( y^{{}\prime}\cdot \frac{\partial F}{\partial y^{\prime}} \right) =  \left(\frac{\partial F}{\partial x} - \frac{\partial F}{\partial x}- \frac{\partial F}{\partial y} \cdot y^\prime \right) + y^{\prime}\cdot \frac{\partial}{\partial x} (\frac{\partial F}{\partial y^{\prime}} )
$$
拆括号化简可得
$$
\frac{\partial}{\partial x} \left( y^{{}\prime}\cdot \frac{\partial F}{\partial y^{\prime}} \right) = \frac{\partial F}{\partial x} - \frac{\partial F}{\partial x} + y^{\prime} \left[\frac{\partial F}{\partial y}- \frac{\partial}{\partial x} (\frac{\partial F}{\partial y^{\prime}} ) \right]
$$
$\left[\frac{\partial F}{\partial y}- \frac{\partial}{\partial x} (\frac{\partial F}{\partial y^{\prime}} ) \right]$实际上就是上面所推导出的欧拉方程，在最优路径上其值为 0，因此该式可化为
$$
\frac{\partial F}{\partial x} - \frac{\partial }{\partial x}(F-y^{{}\prime}\cdot \frac{\partial F}{\partial y^{\prime}})=0
$$
这就是另一种欧拉方程的形式。在某些情况下若能给定$\frac{\partial F}{\partial x}=0$，这意味着$x$并不显含于$F$（也就是$F(x,y,y')$实际可能是$F(y,y')$，$x$ 仍隐含于$F$），所有其他项在关于$x$偏微分时都视为常数，也就是说$F-y^{{}\prime}\cdot \frac{\partial F}{\partial y^{\prime}}$是一个常数$c$。
$$
F-y^{{}\prime}\cdot \frac{\partial F}{\partial y^{\prime}}=C
$$