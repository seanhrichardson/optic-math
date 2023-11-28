---
layout: page
title: Manifolds
---
<!-- 
pre reqs: 
- basic topology
- subspace topology
-->


<!-- TODO:
This is written for Riemannian manifolds, but this can be greatly shortened if the goal is only topological manifolds. -->

## Manifolds

/\*examples\*/

All of the above examples have one important property: a neighborhood each point \\(p\\) of an \\(n\\) dimensional manifold \\(M \subset \mathbb{R}^m\\) must look locally like \\(\mathbb{R}^n\\); we call this property *locally Euclidean*. Note we can consider a manifold \\(M \subset \mathbb{R}^m\\) as a topological space by using the subspace topology, so we can use the following formal definition of locally Euclidean.

**Def. (Locally Euclidean).** A topological space \\(X\\) is *locally Euclidean of dimension \\(n\\)* if for each \\(p \in X\\), there exists an open set \\(U \subset X\\) containing \\(p\\) that is homeorphic to an open subset \\(U \subset \mathbb{R}^n\\).

With this definition in hand, we can give a formal definition of manifold.

**Def. (Manifold).** A subset \\(M \subset \mathbb{R}^m\\) is called an *\\(n\\)-dimensional manifold* if \\(M\\) is locally Euclidean of dimension \\(n\\).

However, while the above definition is what /\*Gauss used? give some history?\*/, it has the limitation of requiring a manifold to be a subset of \\(\mathbb{R}^m\\) for some \\(m\\). Instead, the modern approach to manifold theory is to define manifolds as mathematical objects in their own right satisfying particular properties, which has a few advantages.

1. All manifolds *can* be realized as subsets of \\(\mathbb{R}^m\\), but for some manifolds, it is unnatatural to do so. The modern definition allows the flexibility to define these manifolds in more convenient ways, we just need to check that it satisfies the necessary properties.
2. When studying theorems that hold for all manifolds, it will be more clear what properties are responsible for the theorem, providing us with a deeper understanding.

In fact, the modern approach defines several different types of manifolds. For example,
* A *topological manifold* is any topological space that could come from a manifold as defined above.
* A *smooth manifold* is a topological manifold with some extra structure that allows us to do calculus on the manifold (for example, differentiating functions on the manifold).
* A *Riemannian manifold* is a smooth manifold with some extra structure that gives the manifold geometry: angles, lenths, areas, etc.

Distinguishing between manifolds with different levels of structure is useful in light of point (2) above: if we prove a theorem for topological manifolds, then only the topology of the manifold is relevant. However, if we prove a theorem for Riemannian manifolds, then the result likely depends on the geometry of the manifold.

However, there is one major disadvantage with this modern approach: if I gave you the formal definitions for topological, smooth, and Riemannian manifolds right now, they would make no sense. Thus we will use slowly build towards these definitions.