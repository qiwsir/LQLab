# 343页结论的证明

证明 $E(\pmb{X}^{\text{T}})=E(\pmb{X})^{\text{T}}$

《机器学习数学基础》的 343 页，有这样一句话：

对于多维随机变量 $\pmb{X}$ ，根据数学期望的定义，有：$E(\pmb{X}^{\text{T}})=E(\pmb{X})^{\text{T}}$ 。

有读者对这句话中的结论不理解，希望能给出有关证明。

证明过程见下。

**证明：**

随机变量 $\pmb{X}$ 是一个向量，于是数学期望可以写成：

$$
E(\pmb{X}) =\begin{pmatrix} E(X_1)\\E(X_2)\\\vdots \\E(X_n)\end{pmatrix}
$$

其中， $X_i$ 是 $\pmb{X}$ 的第 $i$ 个分量。

$\pmb{X}$ 的转置 $\pmb{X}^{\text{T}}$ ，如果用分量的形式，可以将 $\pmb{X}$ 写成：$\pmb{X}=(X_1,X_2,\cdots,X_n)^{\text{T}}$ ，也就是有：$\pmb{X}^{\text{T}}=(X_1,X_2,\cdots,X_n)$ 。于是：

$$
E(\pmb{X}^\text{T}) = \begin{pmatrix} E(X_1) & E(X_2) & \dots & E(X_n) \end{pmatrix}
$$

再对 $E(\pmb{X})$ 求转置，则得到：

$$
E(\pmb{X})^\text{T} = \begin{pmatrix} E(X_1) \\ E(X_2) \\ \vdots \\ E(X_n) \end{pmatrix}^\text{T} = \begin{pmatrix} E(X_1) & E(X_2) & \dots & E(X_n) \end{pmatrix}
$$


比较上述两个式子，于是得到结论：

$$
E(\pmb{X}^{\text{T}})=E(\pmb{X})^\text{T}
$$

证毕。