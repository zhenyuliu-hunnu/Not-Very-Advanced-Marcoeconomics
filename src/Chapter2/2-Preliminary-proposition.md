# 预备定理

在进入变分法前需要先了解下面这个定理，这个定理非常直观，很好理解，这里也会给出非常简洁的代数证明。

## 定理

对于函数$M(x)$ 和任意满足$h(a)=h(b)=0$的函数 $h(x)$ ，若有
$$
\int_{a}^{b} M\left( x \right) h\left( x \right) dx=0
$$
那么
$$
M(x)=0
$$

## 证明

令$h(x)=-M(x)(x-a)(x-b)$，其满足$h(a)=h(b)=0$。

代入得
$$
\int_{a}^{b} M\left( x \right) h\left( x \right) dx=\int_{a}^{b} M\left( x \right) \cdot -M(x)(x-a)(x-b)) =\int_{a}^{b}M^2(x)(-(x-a)(x-b))dx=0
$$
易知在$(a,b)$区间$-(x-a)(x-b)>0$，若要使得该式成立，那么一定有$M^2(x)=0$，所以可以得到
$$
M(x)=0
$$