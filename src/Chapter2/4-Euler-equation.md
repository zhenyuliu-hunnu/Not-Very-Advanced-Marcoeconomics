# 欧拉方程的推导

欧拉方程的成就，在于把前面不可操作的微分形式变得可操作。接下来的内容就是欧拉方程的推导。

## 回到泛函

根据定义，最优路径就是使得路径用时$T[y(x)]$最小的路径。任何路径必将经过某个$x$区间，因此路径的总值就是这些区间内路径的加总。根据微积分的思想，在连续时间情形下，$x_1$ 到 $x_2$ 区间的路径就是一个定积分。

在连续的路径上找到某个时刻的「路径」，我们需要三部分信息：开始阶段、开始状态、「路径」方向。由于每条「路径」都是无限小的，因此三部分信息可以表示为$x, y(x), y'(x)$。如果存在某个函数$F$可以将这三个量转化为「路径」的值，那么某一路径$A$在某一时刻$x_0$的值可以写为$F[x_0, y_A(x_0), y'_A(x_0)]$。所以整个泛函可以被改写为
$$
T[y]=\int_{0}^{x} F[x, y(x), y'(x)]dx
$$

## 从泛函到函数

有了上面的式子，加上前面对于可行路径的定义，前面的关于$\varepsilon$的函数$I(\varepsilon)$ 就可以写为
$$
I(\varepsilon)=\int_{0}^{X} F[x,y^*+\varepsilon \eta,y^{*\prime}+\varepsilon \eta'] dx
$$
为了简化表达，这里将函数写成了变量。

我们最终的目标是
$$
\left.\frac{dI}{d\varepsilon}\right|_{\varepsilon=0} = 0
$$
被积的变量是 $x$，根据莱布尼兹法则，我们可以穿过积分符号对$\varepsilon$进行求导。
$$
\frac{dI}{d\varepsilon} = \int_{0}^{X} \frac{dF}{d\varepsilon}dx {{numeq}}
$$


## 全微分

为了简化过程，我们令$$
u = y^*+\varepsilon \eta \quad v=y^{*\prime}+\varepsilon \eta'
$$
被积函数即为$F(x,u,v)$，根据全微分公式有
$$
\frac{\partial F}{\partial \varepsilon} =\frac{\partial F}{\partial x} \cdot \frac{\partial x}{\partial \varepsilon} +\frac{\partial F}{\partial u} \cdot \frac{\partial u}{\partial \varepsilon} +\frac{\partial F}{\partial v} \cdot \frac{\partial v}{\partial \varepsilon}
$$
显然，第一项为 0，后两项又有
$$
\frac{\partial u}{\partial \varepsilon} =\eta \quad \frac{\partial v}{\partial \varepsilon} =\eta'$$
因此
$$
\frac{\partial F}{\partial \varepsilon} =\frac{\partial F}{\partial u} \cdot \eta +\frac{\partial F}{\partial v} \cdot \eta^{\prime}
$$
(2.4.1)变为
$$
\frac{dI}{d\varepsilon} = \int_{0}^{X} (\frac{\partial F}{\partial u} \cdot \eta +\frac{\partial F}{\partial v} \cdot \eta^{\prime})dx {{numeq}}
$$

## 极值点

现在让$\epsilon =0$，注意到，此时$u=y^{*},v=y^{* \prime}$，所以
$$
\left.\frac{dI}{d\varepsilon}\right|_{\varepsilon=0} = \int_{0}^{X} (\frac{\partial F}{\partial y^*} \cdot \eta +\frac{\partial F}{\partial y^{* \prime}} \cdot \eta^{\prime})dx =0
$$
利用积分的性质，被积函数第一项暂且不看，先看第二项，注意$\eta$是关于$x$的函数，所以可以写为
$$
\int_{0}^{x} \frac{\partial F}{\partial y^{* \prime}} \cdot \frac{\partial \eta}{\partial x}dx =\int_{0}^{x} \frac{\partial F}{\partial y^{* \prime}}  d \eta
$$
这时候就可以使用分部积分法$\int u dv = uv - \int vdu$求积分。
$$
\int_{0}^{X} \frac{\partial F}{\partial y^{* \prime}}  d \eta= \left.\eta \frac{\partial F}{\partial y^{* \prime}} \right|^{X}_{0} -\int_{0}^{X}   \eta \frac{\partial }{dx}(\frac{\partial F}{\partial  y^{* \prime}})
$$
由于$\eta(x)$和最优路径有相同的起点和终点，因此第一项显然为 0。代回原式可得：
$$
\left.\frac{dI}{d\varepsilon}\right|_{\varepsilon=0} = \int_{0}^{X} (\frac{\partial F}{\partial y^*} \cdot \eta -\eta \frac{\partial F_{y^{* \prime}}}{dx})dx =\int_{0}^{X} \eta[\frac{\partial F}{\partial y^*}-\frac{\partial F_{y^{* \prime}}}{dx}]=0
$$
现在我们可以使用 2.2 中的定理了。要使得这个微分结果为0，这意味着有
$$
F_{y^{*}}-\frac{\partial }{dx}F_{y^{* \prime}}=0  \quad t\in[x_1,x_2]
$$

这就是欧拉方程（Euler equation），它就是极值路径的一个必要条件。

> [!Important]
>
> 欧拉方程不依赖任何具体表达式，因此一旦给定可微函数$F(x,y,y^\prime)$，就都可以对其使用欧拉方程。
