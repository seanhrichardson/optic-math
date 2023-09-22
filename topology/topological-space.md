---
layout: page
title: Topological Spaces
---

## Topological Spaces

#### Motivation
Recall that a metric space \\((X,d)\\) has the following notion of an *open set*. We say \\(U \subset X\\) is open if for all \\(x \in U\\), there exists some \\(\varepsilon > 0\\) such that the open ball \\(\\{x': d(x,x') < \varepsilon\\}\\) is a subset of \\(U\\). These open sets are most useful in providing an alternate definition of continuity. In particular,

*A function \\(f: X \to Y\\) between two metric spaces is continuous if and only if for each open set \\(U \subset Y\\), the preimage \\(f^{-1}(U)\\) is open.*

That is, we only need to know the open sets to understand continuous functions. The field of topology asks the question: what else can we do using *only* the open sets. In addition to continuity, we can also define convergence of sequences, compactness,  connectedness, and many other concepts using only open sets. This generalizes these notion into spaces that do not necessarily even have a metric. Instead of studying metric spaces, topology studies *topological spaces* -- sets in which we know what the open sets are. 

#### Definition

**Def.** A *topological space* is any space \\(X\\) together with a collection \\(\mathcal{T}\\) of subsets of \\(X\\), called the *open sets* of \\(X\\), that satisfy the following properties.
1. The union of arbitrarily many open sets is open. That is, if \\(\\{U\_{\alpha}\\}\_{\alpha \in A} \subset \mathcal{T}\\), then \\(\bigcap_{\alpha \in A}U_{\alpha} \in \mathcal{T}\\).
2. The intersection of finitely many open sets is open. That is, if \\(U_1, \cdots, U_n \subset \mathcal{T}\\), then \\(U_1, \cdots, U_n \in \mathcal{T}\\).
3. The emptyset is open, and the entire space is open. That is, \\(\emptyset, X \in \mathcal{T}\\).

Note the open sets of a metric space satisfy properties (1), (2), and (3), but we will discuss these properties after the following definition of continuity.

**Def.** Let \\(f: X \to Y\\) be a map between two topological spaces. Then, \\(f\\) is *continuous* if for every open subset \\(U\\) of \\(Y\\), the set \\(f^{-1}(U)\\) is an open subset of \\(X\\).

Defining continuity like this should come as no surprise: it is this property that motivates the idea of topological spaces. 

/\*TODO: exercise... consider \\(f: X \to Y\\) for \\(Y\\) a metric space... use preimages to motivate (1), (2), (3) somehow... this should be an extension of notion of continuity, so needs to play nicely with metric spaces.\*/

#### Examples

/\*\\(\mathbb{R}^n\\)\*/

/\*\\(S^n\\)\*/

/\*Any metric space\*/

#### Closed Sets

**Def.** Given a topological space \\(X\\), a subset \\(A \subset X\\) is called *closed* if its complement is open.

**Prop.** A map \\(f: X \to Y\\) is continuous if and only if for every closed subset \\(A\\) of Y, the set \\(f^{-1}(A)\\) is a closed subset of \\(X\\).

/\*TODO.\*/