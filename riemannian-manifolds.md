---
layout: page
title: Riemannian Manifold
---

## Riemannian Metric on the Sphere

#### Parametrization
TODO: use the word parametrization somewhere
TODO: use the word chart somewhere
TODO: use the word map somewhere

Given a particular surface, our goal is to somehow describe the geometry of that surface. For example, let's begin by considering a sphere.

TODO: insert picture of sphere that we can rotate. (maybe overlaid with Earth map)

The first step in describing the geometry of the sphere is finding a way to communicate different points on the sphere with numbers. One way of doing this is with two angles: latitude and longtitude. We will construct a way of associating points on the sphere with two numbers by taking inspiration from latitude and longtitude.

TODO: insert picture of sphere with latitude and longtitude

As in the figure above, we associate each point on the sphere with two angles $\theta$ and $\phi$. TODO: describe roles of $\theta$ and $\phi$. 

Therefore each pair $\theta, \phi$ corresponds to a unique point on the sphere so long as $0 < \theta < 2\pi$ and $0 < \phi < \pi$. In other words, we have a function $T: (0, 2\pi) \times (0,\pi) \to S^2$ where $T$ takes as input a pair $\theta, \phi$ and outputs the corresponding point on the sphere. Functions such as $T$ are often referred to as "maps"; the following visual of $T$ explains this terminology:

TODO: insert picture of chart to surface with world map.

TODO: explain formula...

\\[T(\theta, \phi) = (\cos\theta\sin\phi, \sin\theta\sin\phi, \cos\phi)\\]

#### Missing information from the map
While the parametrization of the sphere is useful in describing points on the sphere, it is missing some crucial information. For example:

1. What is the angle between two vectors on the chart?
1. What is the length of a vector on the chart?
1. What is the length of a line segment on the chart?
1. What is the area of a region on the chart?
1. What is the distance between two points?
1. How do we know if a line is straight?

TODO: give some examples indicating that none of these are obvious from the map.

The problem is that while the chart provides a way of describing points on the sphere, it contains no information about the *geometry* of the sphere.

INCLUDE?
The same rectangular chart could be used to parametrize a cone, etc....


#### (Tangent) Vectors
TODO: give some description of tangent vectors.

TODO: talk about basis for tangent vectors

TODO: remind reader of formulas for lengths and angles between vectors?

#### Riemannian Metric
Given two vectors $v$ and $w$ based at some coordinates $(\theta, \phi)$ in the chart, the "correct angle" between $v$ and $w$ is the angle between the vectors $DT(v)$ and $DT(w)$. Similarly, the "correct length" of $v$ is the length of the vecor $DT(v)$.

TODO: interactive thing for angles. Ability to move vectors on chart and see angle on sphere.

TODO: interactive thing for lengths.

TODO: emphasize this idea of "pushing forward" more?

Recall that if we can deduce length of vectors and angles between vectors from a dot produc, so to correctly define lengths and angles all we need to do is define the "correct dot product" between the vectors at that point. If $v$ and $w$ are vectors based at the coordinte $(\theta, \phi)$, the "correct dot product" between $v$ and $w$ is the dot product between $DT(v)$ and $DT(w)$!

Defining such a dot product at *every* coordinate point $(\theta, \phi)$ is the fundamental idea of Riemannian geometry. If $v$ and $w$ are vectors at point $(\theta, \phi)$, the "correct dot product" between $v$ and $w$, denoted $g(v,w)$ is
\\[g(v,w) = DT_{(\theta,\phi)}(v) \cdot DT_{(\theta,\phi)}(w)\\]

For pratice, let's compute this inner product for the basis vectors $\{\partial_\theta, \partial_\phi\}$ at each point. 

TODO: make this exercise and hide it?

We need to compute the Jacobi matrix $DT_{(\theta, \phi)}$ at each point.

**Exercise**: ...........

\\[DT =
\begin{pmatrix}
    \frac{\partial x}{\partial \theta} & \frac{\partial x}{\partial \phi}\\
    \frac{\partial y}{\partial \theta} & \frac{\partial y}{\partial \phi}\\
\end{pmatrix}
\\]

\\[g(\partial_\theta, \partial_\phi) = \\]

#### Using Riemannian Metric
TODO: discuss angles between vectors, lengths of vectors, lengths of lines, area of regions.

#### Properties of Riemannian Metric


#### NEXT: define general Riemannian manifold... mew page?