---
layout: page
title: Curvature
---

## Riemann Curvature Tensor

#### Motivation

An important problem in Riemannian geometry is given two Riemannian manifolds, when are they isometric? A first step to answering this question is to determine when two points on different Riemannian manifolds have neighborhoods that are isometric. This is still a hard problem to answer in general, but an easier question is: when does a point on a Riemannian manifold have a *flat neighborhood* (a neighborhood isometric to a neighborhood of \\(\mathbb{R}^n\\))? We will now investigate this question and try to identify the obstruction to a neighborhood being flat.

/\*give motivation for faillure of Hessian to commute.\*/

#### Flatnness Criterion

**Thm (Flatnness Criterion).** A neighborhood \\(U\\) of a Riemannian manifold \\(M\\) is flat if and only if \\(\nabla^2\_{X,Y} Z - \nabla^2\_{Y,X} Z \equiv 0\\) over \\(U\\).

*Proof.* /\*TODO\*/

#### Riemann Curvature Tensor.

We have seen that coordinate-invariant tensor given by the difference of Hessians \\(\nabla^2\_{X,Y} Z - \nabla^2\_{Y,X} Z\\) contains the important geometric information of whether the metric is locally flat about a point. We will see that this tensor \\(\nabla^2\_{X,Y} Z - \nabla^2\_{Y,X} Z\\) contains much more important geometric information such as how geodesics diverge or converge and the commutativity of parallel transport. This extremely important tensor warrants a definition.

**Def (Riemann Curvature Tensor).** The *Riemann curvature tensor* is the \\((3,1)\\) tensor \\(R(X,Y)Z := \nabla^2\_{X,Y} Z - \nabla^2\_{Y,X} Z\\).

We will first study how the Riemann curvature tensor encodes the (non)-commutativity of parallel transport, for this yields a nice geometric and visual interpretation of the Riemann curvature tensor. 

#### Noncommutativity of Parallel Transport

/\*describe the intuition...\*/

/\*maybe replace with \\(\delta\\) and \\(\varepsilon\\)\*/ /\*explain below more\*/

/\*maybe make the below argument visually as intuition\*/

\\[
\begin{align}
    &P\_\{(S,T)}^\{(S,0)} P\_\{(S,0)}^\{(0,0)} X\_{(0,0)} - P\_\{(S,T)}^\{(0,T)} P\_\{(0,T)}^\{(0,0)}X\_{(0,0)}\\\\\
    &= ((X\_{(S,T)} - P\_\{(S,T)}^\{(0,T)}X\_{(0,T)})
    - P\_\{(S,T)}^\{(S,0)}(X\_{(S,0)} - P\_\{(S,0)}^\{(0,0)}X\_{(0,0)}))\\\\\
    &- ((X\_{(S,T)} - P\_\{(S,T)}^\{(S,0)}X\_{(S,0)})
    - P\_\{(S,T)}^\{(0,T)}(X\_{(0,T)} - P\_\{(0,T)}^\{(0,0)}X\_{(0,0)}))\\\\\
    <!-- roughly equal to... (not exact because of parallel transport) -->
    &\approx \int\_{0}^S (D_s X)\_{(s,T)} ds - \int\_{0}^S (D_s X)\_{(s,0)} ds 
    - \left(\int\_{0}^T (D\_t X)\_{(S,t)} dt - \int\_{0}^T (D\_t X)\_{(0,t)} dt\right)\\\\\
    &= \int\_{0}^S \int\_{0}^T (D\_tD\_s X)\_{(s,t)} dt ds
    -  \int\_{0}^T \int\_{0}^S (D\_tD\_s X)\_{(s,t)} ds dt\\\\\
    &= \int\_{0}^S \int\_{0}^T (D\_tD\_s X)\_{(s,t)} - (D\_sD\_t X)\_{(s,t)} dt ds\\\\\
    &\approx st (D\_tD\_s X - D\_sD\_t X)\_{(0,0)}
\end{align}
\\]

**Thm (Curvature and Parallel Transport).** /\*todo\*/

*Proof.* /\*TODO\*/