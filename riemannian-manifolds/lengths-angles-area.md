---
layout: page
title: Lengths, Angles, Area
---

## Lengths, angles, and areas

Given a Riemannian manifold \\(M\\), its Riemannian metric \\(g\\) encodes key *geometric* information about the manifold. For example, below are some key geometric questions that the metric allows us to answer.

1. Given two intersecting curves \\(\alpha, \beta: [0,1] \to M\\), what is the angle of their intersection?
2. What is the length of a curve \\(\gamma: [0,1] \to M\\)?
3. Given a region \\(\Sigma \subset M\\) of the manifold, what is the area or volume of the region?
4. Given two points \\(p,q \in M\\), what is the distance between \\(p\\) and \\(q\\)?
5. Given a curve \\(\gamma: [0,1] \to M\\), how do we know if it is straight?

On this page we will show how the Riemannian metric allows us to answer (1), (2), and (3).

#### Angles

/\*could make this more "precisely motivated" by comparing to extrinsic embeded Riemannian manifolds...\*/

Suppose we have two smooth curves \\(\alpha: [a\_0, a\_1] \to M\\) and \\(\beta: [b\_0, b\_1] \to M\\) that intersect at \\(\alpha(\widetilde{a}) = p = \beta(\widetilde{b})\\). Then what angle do they intersect at? The motivation behind the definition of the Riemannian metric is that we define this angle to be the angle between the *tangent vectors* \\(\alpha'(\widetilde{a}), \beta'(\widetilde{b}) \in T\_pM\\). The Riemannian metric \\(g\\) offers an inner product on \\(T\_pM\\) which, like any inner product, gives a notion of angles. In particular, the angle \\(\theta\\) between \\(\alpha'(\widetilde{a}), \beta'(\widetilde{b})\\) is given by
\\[
    \cos\theta = \frac{\langle \alpha'(\widetilde{a}) , \beta'(\widetilde{b}) \rangle\_g}{\|\alpha'(\widetilde{a})\|_g \|\beta'(\widetilde{b})\|_g}.
\\]
We consider this angle \\(\theta\\) given above to be the angle thata the curves \\(\alpha\\) and \\(\beta\\) intersect at.

#### Lengths

What is the length of a smooth curve \\(\gamma: [a,b] \to M\\)? /\*compare to extrinsic case...\*/


