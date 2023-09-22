---
layout: page
title: Spectral Theorm for Matrices
---

## Spectral Theorem

#### Statement
Let \\(T: V \to V\\) be Hermitian. Then \\(V\\) has an orthornomal basis of eigenfunctions of \\(T\\).

/\*TODO: expand on the below in places... (perhaps with optional hidden expansions)\*/

/\*TODO: Maybe use \\(T\\) instead of \\(A\\) below?\*/

/\*Use ideas in last paragraph to motivate why symmetry is so important.\*/
#### Proof
Note that by \\(T\\) Hermitian, the inner product \\(f(x) = \langle Tx , x\rangle\\) is real. Therefore, by continuity and compactness, the image \\(f(\\{x: \\|x\\| = 1\\})\\) has some maximum \\(f(y)\\). 

By Lagrange's multiplier theorem, such a vector \\(y\\) must satisfy \\(\nabla (y^{\dagger}Ty) = \nabla (y^{\dagger} y)\\).

Therefore, using the product rule, we find that for all \\(z \in V\\).
\\[\begin{align}
0 = \langle \nabla (y^{\dagger}Ty) - \nabla (y^{\dagger} y) , z \rangle 
= \cdots
= 2z^{\dagger}\left(\frac{T+T^{\dagger}}{2}y - \lambda y\right).
\end{align}\\]

Thus \\(\frac{1}{2}(T+T^{\dagger})y = \lambda y\\) and so by \\(T\\) Hermitian, \\(Ty = \lambda y\\).

Now let \\(E\\) be the eigenspace of \\(\lambda\\), decompose \\(V = E \oplus E^{\perp}\\), and consider the restricted operator \\(T: E^{\perp} \to V\\). If we can show \\(T(E^{\perp}) \subset E^{\perp}\\), then the theorem follows by repeating the argument for \\(T: E^{\perp} \to E^{\perp}\\) and inducting. Indeed, we have \\(T(E) \subset E\\) by \\(E\\) the eigenspace of \\(\lambda\\). Therefore, for any \\(x \in E^{\perp}\\) and \\(z \in E\\) we find, using \\(T\\) is Hermitian, \\(\langle Tx , z \rangle = \langle x , Tz\rangle = 0\\) and so \\(Tx \in E^{\perp}\\).

