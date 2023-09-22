---
layout: page
title: Riemannian Manifolds
---

## Smooth Manifolds

Previously on /\*this page\*/, we developed a method for computing the lengths of lines, angles between lines, and areas of regions on the sphere. The steps to this method are as follows...

/\*explain steps for one chart, but mention things get more complicated for more charts\*/

These methods will likely work for any surface you come accross, 

#### Coordinate Charts
Given any \\(n\\)-dimensional surface \\(M\\), we want to parametrize it using coordinate charts \\(\varphi_{k}: U_{k} \to M\\) that satisfy a few rules.

1. Each \\(U_{k}\\) is a subset of \\(\mathbb{R}^n\\). This allows it to provide coordinates.
1. Each coordinate chart \\(\varphi_{k}\\) is a bijection. This allows for every point on the coordinate chart to correspond to a unique point on the surface.
1. The images of all coorinate maps \\(\varphi_k\\) cover the entire surface. /\*motivate\*/

/\*break... talk about the aboe\*/

/\*figure out how to continue numbering...\*/

/\*maybe give smooth transition maps more emphasis? Could motivate this with the sphere?\*/

1. There are only countably many coordinate charts \\(U_k\\).
1. Each chart \\(U_{k}\\) is open in \\(\mathbb{R}^n\\). This ensures that every point in the chart has a small neighborhood around it /\*explain why this is useful\*/.
1. The intersections \\(\varphi_k(\varphi_k(U_k) \cap \varphi_l(U_l))\\) and \\(\varphi_l(\varphi_k(U_k) \cap \varphi_l(U_l))\\) are open in \\(\mathbb{R}^n\\). /\*motivate: either sequence counterexample or next property\*/
1. The transition maps \\(\varphi_l^{-1} \circ \varphi_k: \varphi_k(\varphi_k(U_k) \cap \varphi_l(U_l)) \to \varphi_l(\varphi_k(U_k) \cap \varphi_l(U_l))\\) are smooth. /\*motivate... often need derivatives here to exist and easiest to ensure infinitely many exist. For example, \*/
1. Any two points \\(p,q\\) in the surface \\(M\\) are either in the same chart, or there exists charts \\(U_k\\) and \\(U_l\\) so that \\(p \in U_k\\), \\(q \in U_l\\), yet \\(\varphi_k(U_k)\\) and \\(\varphi_l(U_l)\\) are disjoint.

/\*Above is a bit overwhelming. Have key points at the beginning, and throw the more complicated relations into the bottom with less emphasis and perhaps optional/hidden explanations.\*/

#### Examples
/\*introduce examples... provide coordinate charts for sphere, torus, euclidean space? Perhaps as exercises?\*/

