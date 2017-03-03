# 多项式

## 多元多项式
### 定义
设 K 为数域， $$x_1, x_2, \cdots , x_n$$ 为未定元， $$a \in K, k_1, k_2, \cdots k_n \in ℤ ≥ 0$$ 为非负整数，称 $$ax_1^{k_1}x_2^{k_2} \cdots x_n^{k_n}$$ 为 **单项式**
	- 若 a≠0，定义 **次数** = $$k_1 + k_2 + \cdots +k_n$$
	- 若 a=0，定义 **次数** = $$-\infty$$
### 同类项加法
有限个单项式的形式和称为 **多项式**
	- $$f(x_1, \cdots x_n) = \sum_\limits{(i_1, \cdots i_n)\in ℤ^n_{≥0}}a_{i_1\cdots i_n}x^{i_1}_1 \cdots x^{i_n}_n$$
### 运算
	- 加法：$$f + g = \sum_\limits{(i_1, \cdots ,i_n)\in ℤ^n_≥0}{(a_{i_1\cdots i_n} + b_{i_1\cdots i_n})x^{i_1}_1 \cdots x^{i_n}_n}$$
	- $$k \in K$$ 数乘：$$f + g = \sum_\limits{(i_1, \cdots ,i_n)\in ℤ^n_≥0}{(ka_{i_1\cdots i_n})x^{i_1}_1 \cdots x^{i_n}_n}$$
	- 乘积：利用分配率化为单项式乘积，再合并同类项进行化简
- $$K[x_1, \cdots ,x_n]$$ 为 K 上的代数，称为 K 上的 n 元 **多项式代数（环）**
	- *命题* 整性： $$f(x) = a_m x^m + a_{m-1} x^{m-1} + \cdots + a_0, a_m ≠ 0 \\ deg(f(x) \cdot g(x)) = degf(x) + degg(x)$$
		- ⇒ 若 f(x)≠0, g(x)≠0，则 f(x)•g(x)≠0
		- 证明：f≠0 ⇒ f 的首项 ≠0, g≠0 ⇒ g 的首项 ≠0
		则 fg 的首项 = f 的首项 × g 的首项 ≠ 0
### 排序 
- **字典排序法**： 将未定元按自然足标（加权）排序。 
- *引理* 设 $$f,g \in K[x_1 \cdots x_n]$$ ，则在字典排序下， fg的首项 = f的首项 × g的首项 
- *推论* 乘法消去律：设 $$f,g,h ≠ 0 \in K[x_1, \cdots x_n]$$ 满足 $$fh = gh$$，则$$f = g$$
### 齐次多项式 
若 $$f(x_1 \cdots x_n)$$ 的所有单项式都是 m 次的，则称 f 为 **m次齐次多项式** 或 **m次型**
- *引理*
	- 设 f≠0 是 m 次齐次多项式，g≠0 是 k 次齐次多项式，则 fg≠0 为 m+k 次齐次多项式
	- **齐次分解（齐次排列）**：设 deg f = d ≥ 0，则 $$f = f_d + f_{d-1} + \cdots + f_0, f_d ≠ 0, f_i$$ 一定是 0 或 i 次多项式
- *命题* 设 $$ f,g \in K[x_1, \cdots ,x_n]$$ 则
	- $$deg(f \cdot g) = deg f + deg g$$
	- $$deg(f+g) ≤ max {deg f, deg g}$$
- **多元多项式** $$f=g$$ 的充分必要条件是 **多元多项式函数** $$f=g$$
	- 必要性：显然
	- 充分性：
		- *引理* 设 $$f(x_1, x_2, \cdots , x_n)$$ 是 K 上的 n 元非零多项式，则 $$\exists a_1, a_2, \cdots a_n \in K, s.t. f(a_1, a_2, \cdots a_n) ≠ 0$$

## 对称多项式
若将某多元多项式的两个指标互换不改变多项式，则此多项式称为 **对称多项式**
### 性质
1. 对称多项式的指标在全排列下不改变
2. 对称多项式的多项式仍然是对称多项式
### 初等对称多项式
$$ \sigma_1 = x_1 +x_2 + \cdots +x_n = \sigma \limits_{i=1}ⁿ x_i \\
\sigma_2 = x_1 x_2 + x_1 x_3 +\cdots x_{n-1}x_n = \sigma \limits_{1≤i<j≤n} x_i x_j \\
\sigma_n = x_1 x_2 \cdots x_n$$

### 对称多项式基本定理
设 $$f(x_1, \cdots x_n)$$ 是数域 K 上的对称多项式，则必存在 K 上的一个多项式 $$g(y_1, \cdots y_n)$$ 使
$$f(x_1, \cdots x_n) = g(\sigma_1, \cdots \sigma_n)$$
*证明*：
- 存在性
构造性证明
引理：设对称多项式字典序下的首项为 $$a x_1 ^{i_1} x_2 ^{i_2} \cdots x_n ^{i_n}, a ≠ 0$$ ，则必有 $$i_1 ≥ i_2 ≥ \cdots ≥ i_n$$ 
以下“程序”
 $$ f_0 = f, f_1 = f_0 - g_1, f_2 = f_1 - g_2, \cdots $$
一定会在有限步之内停止，存在性得证

- 唯一性
反证法

### 求对称多项式表示
待定系数法