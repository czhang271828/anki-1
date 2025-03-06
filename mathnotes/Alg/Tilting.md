# 斜置理論 (Tilting Theory): 僅是導引

## Sec 1 

Torsion pair. 

爲研究複雜環 $A$, 有時可以尋找一類斜置模 $T_A$, 使得 $\mathrm{End}(T_A)$ 是較爲簡單的代數, 同時 $𝐦𝐨𝐝 _A$ 與 $𝐦𝐨𝐝 _B$ 等價. 如[此文](https://link.springer.com/chapter/10.1007/978-94-017-1556-0_9)之定理 (5). 

Useful references. 
1. [First 20 years of Tilting](https://webusers.imj-prg.fr/~bernhard.keller/publ/dctabs.html)
2. [Collection of notes](https://www.maths.ed.ac.uk/~v1ranick/papers/tilting.pdf)
3. 

Torsion pair, Tilting module. 


%

## 擾對 (Torsion pair)

**定義** 稱 $(ℱ, 𝒯)$ 是 擾對, 當且僅當 $𝒯 ⟂_{\mathrm{Hom}} ℱ$, 且 $𝒯 ^{⟂ ⟂ } = 𝒯$, $ℱ^{⟂ ⟂ } = ℱ$. 

1. $ℱ$ 稱作 torsion-free class; 
2. $𝒯$ 稱作 torsion class. 

**案例** 一些基本的構造. 

1. (得名緣由) 例如 $𝒯$ 是有限 Abel 群, $ℱ$ 是有限生成自由 Abel 群. 
2. 給定對象類 $𝒳$, 則 $(𝒳^{⟂}, {^⟂}(𝒳^⟂)$ 與 $((^⟂ 𝒳)^⟂ , {^⟂ }𝒳 )$ 是擾對. 
3. 給定 $A$ 的擾對 $(ℱ, 𝒯 )$, 則有 $DA$ 的擾對 $(D𝒯, Dℱ )$. 

**重要注记** 从 AR Quiver 的例子来看, 通常有若干对 $ℱ → 𝒯$. 

%

## 擾對對應 $t$-函子

**定義** 稱 $t$ 是 radical 函子, 當且僅當 $t$ 是 $\mathrm{id}$ 的子函子, 且
$$
0 → tM → M → M / tM → 0
$$
在函子 $t$ 的作用下是 
$$
0 → tM = tM → 0 → 0. 
$$

- **標語** radical 函子是函子行爲像 $\mathrm{Rad}$ 的函子. 

**定理** $𝒯$ 的等價判別. 以下命題等價. 
1. 存在擾對 $(ℱ , 𝒯)$; 
2. $𝒯$ 對餘極限 (商 + 餘積), 以及擴張封閉; 
3. 存在 radical 函子 $t$ 使得 $t|_𝒯 = \mathrm{id}$. 

**定理** $ℱ$ 的等價判別. 以下命題等價. 
1. 存在擾對 $(ℱ , 𝒯)$; 
2. $ℱ$ 對極限 (子 + 積), 以及擴張封閉; 
3. 存在 radical 函子 $t$ 使得 $t|_ℱ = 0$. 

**命題** 給定 $(ℱ, 𝒯)$ 即是給定 radical 函子 $t$. 任意模 $M$ 均有**同構下唯一**的分解

$$
0 → tM → M → M/tM → 0.
$$

- **標語** 擾模的商, 歸納均是擾模; 無擾模的子, 投射均是無擾模. 

%

## 可裂擾對

**定義** 稱 $(ℱ, 𝒯)$ 可裂, 當且僅當以下等價條件成立. 

1. $𝒯 ⟂_{\mathrm{Ext}^1} ℱ$. 
2. $ℱ$ 關於 $τ$ 封閉. 
3. $𝒯$ 關於 $τ⁻¹$ 封閉. 

**註釋** 此時, 對象類就是 $ℱ ⊕ 𝒯$. 有时记作 $ℱ ∨ 𝒯$. 

%

## Gen (滿) = 像可達, Cogen (單) = 弱拓撲可辨

**定理** 稱 $M ∈ \mathrm{Gen}(T)$, 當且僅當以下等價條件成立. 
1. 存在 $d ≥ 0$ 使得有滿射 $T^d ↠ M$. 
2. $(T, M) ⊗_{\mathrm{End}(T)} T → M,\ ∑ f⊗ x ↦ ∑ f(x)$ 是滿射. 

* $⊗_{\mathrm{End}(T)}$ 表示 $(f ∘ g) ⊗ x = f ⊗ g(x)$. 

- **標語** $M$ 能通過 $T$ 與等價關係描述, 當且僅當 **$M$ 能被 $T$ 的像有限地逼近**. 

**定理** 稱 $M ∈ \mathrm{Cogen}(T)$ 當且僅當以下等價條件成立. 
1. 存在 $d ≥ 0$ 使得有單射 $M ↪ T^d$. 
2. $M → ((M,T),T)_{\mathrm{End}(T)}, \ m ↦[g ↦ g(m)]$ 是單射. 

- **標語** $M$ 能嵌入有限的 $T$, 當且僅當 $M$ 能被所有 $(M → T)$ 區分. 

%

## 子範疇的投射與內射對象

**定義** 稱 $P$ ($I$) 在**子對象類**或全子範疇 $𝒞$ 中投射 (內射), 當且僅當 $\mathrm{Ext}^1(P,-)|_{𝒞} = 0$ ($\mathrm{Ext}^1(-,I)|_{𝒞} = 0$). 

**重要提示** 此處僅是特殊的相對投射於相對內射. 畢竟 $P$ 與 $I$ 需要在 $𝒞$ 中. 

**定理** 以下給出 $\mathrm{Gen}(T)$ ($\mathrm{Cogen}(T)$) 構成 torsion (torsion-free) part 的充分條件. 

1. 若 $T$ 相對 $\mathrm{Gen}(T)$ 投射, 則 $\mathrm{Gen}(T) = 𝒯$. 
2. 若 $T$ 相對 $\mathrm{Cogen}(T)$ 內射, 則 $\mathrm{Cogen}(T) = ℱ$. 

**定理** 若局限於單一的 $𝒯$ 或 $ℱ$, 哪些對象是相對投射 (內射) 的? **以下假定 $M$ 不可分解.**

1. $M ∈ 𝒯$ 相對投射, 當且僅當 $τ M ∈ ℱ$; 
2. $M ∈ 𝒯$ 相對內射, 當且僅當 $M ≃ t(I)$, $I ∉ ℱ$ 是內射對象; 
3. $M ∈ ℱ$ 相對內射, 當且僅當 $τ ⁻¹ M ∈ 𝒯$; 
4. $M ∈ ℱ$ 相對投射, 當且僅當 $M ≃ P / t(P)$, $P ∉ 𝒯$ 是投射對象. 

%

## 忠實模 

**定義** 稱 $M$ 是忠實的, 若以下等價命題成立:

1. $A ↪ \mathrm{End}(M)$ 是單射;
2. 右乘不同的 $A$ 給出不同的態射; 
3. $\mathrm{Ann}_A(M)$ 是零理想; 
4. $A ∈ \mathrm{Cogen}(M)$; 
5. $DA ∈ \mathrm{Gen}(DM)$. 

%

## 局部斜置模: $(ℱ,𝒯) = (\mathrm{Cogen}(τ T), \mathrm{Gen}(T))$ 

**定義** 稱 $T$ 是局部斜置 (partial tilting) $A$-模, 若 
1. $p.\dim T ≤ 1$; 
2. $\mathrm{Ext}^1(T,T)=0$. 

**命題** 局部斜置模與擾對. 
1. $\mathrm{Ext}^1 (T, -)$ 在全子範疇 $\mathrm{Gen}(T)$ 中投射. 
2. $\mathrm{Gen}(T)$ 是擾對的 $𝒯$-部分.
3. $\mathrm{Cogen}(τ T)$ 是擾對的 $ℱ$ 部分.

- **標語** 局部斜置模: $T$ 與 $τ T$ 對稱地出現, $𝒯$ 與 $ℱ$ 對稱地出現. 

%

## 局部斜置模 $→$ 斜置模

**定義** 稱局部斜置模 $T$ 是斜置 (tilting) 的, 當且僅當 $T$ 與 $A$ 有相同的不可分解直和項. 

* 等價地, $A ∈ \mathrm{Cogen}(T)$. 

**注釋** 局部: 不可分解對象未必足夠全面. 

**定理** (Bongartz) 局部斜置模可以補全爲斜置模. 對局部斜置模 $T$, 存在 $E$ 使得 $T ⊕ E$ 斜置. 

**命題** 局部斜置模 $T$ 是斜置模, 當且僅當以下等價命題成立. 

1. $\mathrm{Add}(T) = \mathrm{Add}(A)$.
2. $A ∈ \mathrm{Cogen} (T)$. 
3. 任何 $M ∈ (T)^{⟂, 1}$ 通過 $T$ 有限表現, 即下一條. 
4. $\mathrm{Gen}(T) = (T)^{⟂, 1}$. 
5. $\mathrm{Cogen}(T) = (τ T) ^{⟂, 0}$. 

**定理** 斜置模 $T$ 誘導了擾對
$$
𝒯 = \mathrm{Gen}(T) = (T)^{⟂, 1}, \ ℱ = \mathrm{Cogen}(τ T) = (T)^{⟂, 0}. 
$$

- **標語** 斜置模: **四種生成, 歸於一種擾對**. 

%

## 斜置模的 Torsion 模判别法

**命題** 給定斜置模. $M ∈ 𝒯$ 當且僅當賦值
$$
(T, M) ⊗_{\mathrm{End}(T)} T → M, \ ∑ f ⊗ x ↦ ∑ f(x)
$$
是**雙射**. 

- **標語** 斜置模類似投射模, 只是 Ext-1 垂直從全範疇遷移至 $(T)^{⟂, 1}$. 

**思考** 斜置模區別於投射模的具體方式? 斜置模另有什麼特殊表現?

%

## Sec 2

Brenner and Butler 的理論: 將 $T$ 視作 ${_B}T_A$ ($B := \mathrm{End}_A(T)$), 引出左右擾對, 最終指向四類對象: 
1. $𝒯 := \mathrm{Gen}(T) = \ker \mathrm{Ext}^1_A(T, -)$,
2. $ℱ := \mathrm{Cogen}(τ T) = \ker \mathrm{Hom}_A(T, -)$, 
3. $𝒳 := D ℱ(_BT) = \ker \mathrm{Hom}_B(-, DT) = \ker (- ⊗ _BT)$, 
4. $𝒴 := D 𝒯(_BT) = \ker \mathrm{Ext}_B(-, DT) = \ker \mathrm{Tor}_1^B (-, T)$. 

這給出兩處範疇等價
$$
\mathrm{Ext}_A^1 (T, -) : ℱ  ↔ 𝒳 : \mathrm{Tor}_1^B(-, T), 
$$
$$
\mathrm{Hom}_A(T, -) : 𝒯 ↔ 𝒴 : (- ⊗ _B T). 
$$

%

## 範疇等價 $𝐚𝐝𝐝 (T) ≃ 𝐩𝐫𝐨𝐣 (\mathrm{End}(T))$

**定理** 給定斜置模 $T$, 則有範疇等價
$$
(T,-)_{A} : 𝐚𝐝𝐝 (T) ≃ 𝐩𝐫𝐨𝐣 (\mathrm{End}(T)), \ M ↦ (T,M)_{\mathrm{End}(T)}. 
$$

特別地, $\ker (T,-)_{A} = ℱ$. 對 $M,N ∈ ℱ$, 恆有
1. $(M,N)_A ≃ ((T,M), (T,N))_B$, 
2. $\mathrm{Ext}^1 (M, N) ≃ \mathrm{Ext}^1((T,M), (T,N))$. 

% 

## $T$ 的左模結構

**定理** $T$ 是斜置 $B^{\mathrm{op}}$ 模. 

**定理** 代數同構

1. (雙模對稱性) $A → \mathrm{End}_B(T)^{\mathrm{op}}$ 是代數同構, 映 $a$ 至右乘 $[t ↦ ta]$. 
2. (中心, 聯通分支) $Z(A) = Z(B)$, 態射是 $a ↦ [t ↦ ta]$. 

%

## BB 大定理

**定理** 存在兩處範疇等價
$$
\mathrm{Ext}_A^1 (T, -) : ℱ  ↔ 𝒳 : \mathrm{Tor}_1^B(-, T), 
$$
$$
\mathrm{Hom}_A(T, -) : 𝒯 ↔ 𝒴 : (- ⊗ _B T). 
$$

%

## 斜置模的混合係數公式

**案例** 假定 $M$ 是 $A$ 模, 且 $X$ 是 $B$ 模, 則有同構
1. $(T,M) ⊗ T ≃ M, \ ∑ f ⊗ t ↦ ∑ f(t)$, 以及
2. $X ≃ (T, X ⊗_B T), \ m ↦ [t ↦ m ⊗ t]$. 

此時得混合係數公式
1. $\mathrm{Tor}_1^B (\mathrm{Hom}_A(T,M), T) = 0$, 
2. $\mathrm{Ext}^1_A(T,M) ⊗ _BT = 0$, 
3. $\mathrm{Hom}_A(T, X) ⊗_B T = 0$, 
4. $\mathrm{Ext}_A^1(T, X ⊗_B T) = 0$. 

- **標語** 混合係數公式: 一處 $⊗$ 一處 $\mathrm{Hom}$, 一處導出一處原, 賦值餘賦值均消散. 

另有 $(ℱ, 𝒯)$ 中的短正合列 
$$
0 → (T, M)_A ⊗_B T → M → \mathrm{Tor}_1 ^B(\mathrm{Ext}_A^1 (T,M), T) → 0. 
$$
以及 $(𝒳, 𝒴)$ 中的短正合列 
$$
0 → \mathrm{Ext}_A^1 (T, \mathrm{Tor}_1 ^B(X, T)) → X → \mathrm{Hom}_A(T, X ⊗ _B T) → 0.
$$

- **標語** 混合正合列: 
    $$
    0 → F ∘ G(-) → (-) → \mathrm L^1F ∘ \mathrm R^1 G (-) → 0, 
    $$
    以及 
    $$
    0 → \mathrm R^1 G ∘ \mathrm L^1 F (-) → (-) → G ∘ F (-) → 0. 
    $$

## Tilting! 

**定理** (返璞歸真定理) 假定 $T$ 是無重數的斜置模 (同構意義下唯一), 則 
1. $𝐝𝐢𝐦 \mathrm{Hom}(T,M) = [\dim (T_1, M) \ \cdots \ \dim (T_n, M)]$; 
2. $𝐝𝐢𝐦 \mathrm{Ext}^1(T,M) = [\dim (N, τ T_1) \ \cdots \ \dim (N, τ T_n)]$. 

- **特別注釋** 以上 (簡單的導出函子) 符合斜置的本意. 

## Sec 3 

更多維度, 更多導出. 暫時緩一會兒. 





