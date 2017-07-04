# Groups

## Laws of Composition
合成法则的一些较为平凡的性质：
    - Associative law $$(ab)c = a(bc)$$
    - Commutative law $$(ab = ba)$$
乘积 *(product)* 的定义：
    1. $$[a_1] = a_1$$
    2. $$[a_1 a_2]$$ 由合成法则给出
    3. For any integer *i* in range $$1 ≤ i < n$$, $$[a_1 \cdots a_n] = [a_1 \cdots a_i] [a_{i+1} \cdots a_n]$$ 
恒等元 *(identity)* 至多有一个；
逆 *(inverse)* 的性质：
    - 若 *a* 有 left inverse *l* **和** right inverse *r*, 则 *a* invertible, $$l = r$$, 为 *a* 的 inverse
    - 若 *a* invertible, 则 *a* 的 inverse 唯一
    - $$(ab)^{-1} = a^{-1}b^{-1}$$
    - *a* 可能有 left inverse **或** right inverse, 同时却 not invertible
    
        e.g. $$N = {1, 2, 3, \cdots}, s(n) = n+1$$, $$l(n) = n-1, if n > 1; l(1) = 1$$

## Groups and Subgroups
群 *(group)* 的定义：
    称集合 *G* 是群，当且仅当
    - $$(ab)c = a(bc), \forall a, b, c \in G$$
    - *G* 包含恒等元 *1*
    - $$\forall a \in G, \exists b \in G\ s.t. ab = 1 \land ba = 1$$
    
阿贝尔群 *(abelian group)* 指合成法则可交换的群 
群的阶 *(order)* 指群中元素的个数，阶有限称为 *finite group*, 阶无限称为 *infinite group*
常见的 infinite abelian group 有：
    - $$\mathbb{Z}^+$$ 整数加法群
    - $$\mathbb{R}^+$$ 实数加法群
    - $$\mathbb{R}^{\times}$$ 实数乘法群（不包含0，因为它没有逆）
    - $$\mathbb{C}^+, \mathbb{C}^{\times}$$ 复数域上的群
    
**Cancellation Law**: 若 $$ab = ac$$ 或 $$ba = ca$$, 则 $$b = c$$

