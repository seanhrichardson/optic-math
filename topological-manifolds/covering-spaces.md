---
layout: page
title: Covering Maps
---

## Covering Maps

<!-- MOTIVATION AND ROUTE 1: COMPUTING FUNDAMENTAL GROUPS OF QUOTIENT SPACES -->

/\*discuss the fundmantal groups of \\(\mathbb{S}^1\\) and \\(\mathbb{T}^2\\) with pictures\*/

We suspect that \\(\pi_1(\mathbb{S}) \simeq \mathbb{Z}\\) and \\(\mathbb{T}^2 \simeq \mathbb{Z}^2\\). However, the proving so would require identifying the loop homotopy classes, which in turn requires proving two loops are *not* homotoptic relative to the base point. However, there is a technique to compute these homotopy classes, which stems from the observation that \\(\mathbb{S}^1 \simeq \mathbb{R}/\mathbb{Z}\\) and we suspect \\(\pi_1(\mathbb{S}) \simeq \mathbb{Z}\\). Similarly, \\(\mathbb{T}^2 \simeq \mathbb{R^2}/\mathbb{Z}^2\\) and we suspect \\(\pi_1(\mathbb{T}^2) \simeq \mathbb{Z}^2\\). This is no coincidence: we will see that the maps \\(q: \mathbb{R} \to \mathbb{S}^1\\) and \\(q: \mathbb{R^2} \to \mathbb{T}^2\\) are instances of *covering maps* and we can learn a lot about the fundamental groups of \\(\mathbb{S}^1\\), \\(\mathbb{T}^2\\), and many other spaces through covering maps.

#### Covering Maps

/\*Study spaces \\(X/G\\) for \\(G\\) some group first. Show this has the following properties (the following properties are the ones needes for proofs and slightly more general... ?)\*/

/\*why do we need connectectivity conditions on \\(E\\)?\*/

**Def (Covering Map).** A surjective continuous map \\(q: E \to X\\) from a connected and locally path connected topological space \\(E\\) to an arbitrary topological space \\(X\\) is a *covering map* if it satisfies the following condition. For all \\(p \in X\\), there must exist a neighborhood \\(U \subset X\\) containing \\(p\\) such that \\(q^{-1}(U)\\) is a disjoint union of connected open subsets of \\(E\\), each of which is mapped homeomorphically to \\(U\\) by \\(q\\).