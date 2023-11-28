---
layout: page
title: Geodesic Equation
---

## Geodesics

One important geometric question still remains unanswered: 

*Given a curve \\(\gamma(t)\\) on a Riemannian manifold, how do we know if it is straight?*

/\*...\*/

#### Energy Functional

Given a curve \\(\gamma(t)\\) over 

#### Straight Lines in the Plane

Consider a curve \\(\gamma(t) = (x(t), y(t))\\) on \\(\mathbb{R}^2\\) with \\(a \leq t \leq b\\). Now we consider a small pertubation \\(\gamma_{\varepsilon}(t)\\) of this curve that still has the same endpoints. One way to write such a small pertubation is \\(\gamma\_{\varepsilon}(t) = ((x(t)+\varepsilon f(t), y(t) + \varepsilon g(t))\\) for any choice of smooth functions \\(f(t)\\) and \\(g(t)\\) that satisfy \\(f(a) = f(b) = 0\\) and \\(g(a) = g(b) = 0\\). This last condition is to ensure \\(\gamma_{\varepsilon}(t)\\) has the same endpoints: \\(\gamma_{\varepsilon}(a) = \gamma(a)\\\) and \\(\gamma_{\varepsilon}(b) = \gamma(b)\\). 

Then

/\*change notation above to go with below\*/

/\*evaluate everything below at \\(t\\)\*/

\\[
\begin{align}
0 = \frac{d }{d \varepsilon} E(\gamma_{\varepsilon})
= \frac{d }{d \varepsilon}\int_a^b \dot{x}^2\_{\varepsilon}(t) + \dot{y}^2\_{\varepsilon}(t)
\end{align}dt
= \int_a^b \frac{d }{d \varepsilon} \dot{x}^2\_{\varepsilon}(t) dt + \int_a^b \frac{d }{d \varepsilon} \dot{y}^2\_{\varepsilon}(t) dt
\\]

First compute
\\[
    \int_a^b \frac{d }{d \varepsilon} \dot{x}^2\_{\varepsilon}(t) dt
    = 2\int_a^b \dot{x}\_{\varepsilon} \frac{\partial^2 x}{\partial t \partial \varepsilon} dt
    = \left.\dot{x}\_{\varepsilon}\frac{\partial x}{\partial \varepsilon}\right\|_a^b - 2\int_a^b \ddot{x}\_{\varepsilon} \frac{\partial x}{\partial \varepsilon} dt
    = - 2\int_a^b \ddot{x}\_{\varepsilon} \frac{\partial x}{\partial \varepsilon} dt
\\]
/\*explain boundary terms\*/

An identical computation shows 
\\[
    \int_a^b \frac{d }{d \varepsilon} \dot{y}^2\_{\varepsilon}(t) dt = - 2\int_a^b \ddot{y}\_{\varepsilon} \frac{\partial y}{\partial \varepsilon} dt.
\\]

Therefore 
\\[
    0 = \int_a^b \ddot{x}\_{\varepsilon} \frac{\partial x}{\partial \varepsilon} dt + \int_a^b \ddot{y}\_{\varepsilon} \frac{\partial y}{\partial \varepsilon} dt
\\]
/\*finish explanation\*/

#### Straight Lines on a Manifold
Studying constant-speed curves \\(\gamma: [a,b] \to M\\) that are critical values of the Energy functional
\\[
    E(\gamma) 
    = \frac{1}{2}\int_{a}^b\|\dot{\gamma}^2\|\_g dt
    = \frac{1}{2}\int_{a}^b g_{ij} \frac{\partial x^i}{\partial t} \frac{\partial x^j}{\partial t}dt
\\]
That is, we require
\\[
    \left.\frac{d E(\gamma_{\varepsilon})}{d \varepsilon}\right\|\_{\varepsilon = 0} = 0.
\\]
The following computation yields an equivalent condition.
\\[
    0 = 2\frac{\partial E(\gamma_{\varepsilon})}{\partial \varepsilon}\\\\\
    = \int_{a}^b \frac{\partial }{\partial \varepsilon}\left(g_{ij}\frac{\partial x^i}{\partial t} \frac{\partial x^j}{\partial t}\right)dt\\\\\
    = 
\\]

/\*FINISH THIS COMPUTATION WHEN GOOD SYSTEM TO EXPLAIN STEPS IN EQUATION IS UP AND RUNNING\*/

Therefore we conclude that for a line \\(\gamma(t) = (x^1(t), \cdots , x^n(t))\\) to be straight, it must satisfy
\\[
    \frac{d^2 x^k}{d t^2} + \sum_{ij} \frac{1}{2} g^{kl} \left(\frac{\partial g_{lj}}{\partial x^i} + \frac{\partial g_{il}}{\partial x^j} - \frac{\partial g_{ij}}{\partial x^l}\right)\frac{d x^i}{d t}\frac{d x^i}{d t} = 0, \quad 1 \leq k \leq n
\\]

#### Definition of Geodesics
A curve \\(\gamma(t)\\) is a *geodesic* if, when written in any local coordinates \\(\gamma(t) = (x^1(t), \cdots, x^n(t))\\), it locally satisfies the *geodesic equations*
\\[
    \ddot{x}^k(t) + \dot{x}^i(t)\dot{x}^j(t)\Gamma_{ij}^k(x(t)) = 0, \quad 1 \leq k \leq n
\\]
where the functions \\(\Gamma_{ij}^k\\) are the *Christoffel symbols* and are given in coordinates by
\\[
    \Gamma_{ij}^k = \frac{1}{2}g^{kl}(\partial_i g_{jl} + \partial_j g_{il} - \partial_l g_{ij})
\\]

#### Example: geodesics on the sphere
Computing geodesics on the sphere. We can express a path \\(\gamma: [a,b] \to \mathbb{S}^2\\) in coordinates by \\(\gamma(t) = (\theta(t), \phi(t))\\). First compute the Christoffel symbols /\*TODO: SHOW (hidden?) COMPUTATIONS FOR THESE\*/

Recall \\(g = d\phi^2 + \sin\phi^2 d\theta^2\\)
\\[\begin{align}
    \Gamma_{\phi\phi}^{\phi} &= 0 \\\\\
    \Gamma_{\phi\theta}^{\phi} &= \Gamma_{\theta\phi}^{\phi} = 0\\\\\
    \Gamma_{\theta\theta}^{\phi} &= -\sin\phi\cos\phi\\\\\
    \Gamma_{\phi\phi}^{\theta} &= 0\\\\\
    \Gamma_{\phi\theta}^{\theta} &= \Gamma_{\theta\phi}^{\theta} = \cot\phi\\\\\
    \Gamma_{\theta\theta}^{\theta} &= 0
\end{align}\\]
Hence the geodesic equations become
\\[
\begin{align}
    \ddot{\theta}(t) + 2\dot{\theta}(t)\dot{\phi}(t)\cot(\phi(t)) &= 0\\\\\
    \ddot{\phi}(t) - \dot{\theta}^2(t)\sin(\phi(t))\cos(\phi(t)) &= 0.
\end{align}
\\]
Observe that the equator \\(\gamma(t) = (t, \pi/2)\\) satisfies the geodesic equations along with any meridian \\(\gamma(t) = (\theta, t)\\) for some constant \\(\theta\\).

In fact, as any great circle on the sphere can be expressed as a meridian (by choosing the north and south pole to be on that great circle), this shows all great circles on the sphere are geoesics!

#### Example: geodesics in hyperbolic space
Computing geodesics in hyperbolic space.

First compute the Christoffel symbols.
\\[\begin{align}
\Gamma_{xx}^x &= 0\\\\\
\Gamma_{xy}^x &= \Gamma_{yx}^x = \frac{-1}{y}\\\\\
\Gamma_{yy}^x &= 0\\\\\
\Gamma_{xx}^y &= \frac{1}{y}\\\\\
\Gamma_{xy}^y &= \Gamma_{yx}^y = 0\\\\\
\Gamma_{yy}^y &= \frac{-1}{y}
\end{align}\\]

Thus the geodesic equations for a curve \\(\gamma(t) = (x(t), y(t))\\) are
\\[\begin{align}
\ddot{x}(t) - \frac{2}{y(t)}\dot{x}(t)\dot{y}(t) = 0\\\\\
\ddot{y}(t) + \frac{1}{y}(\dot{x}(t)-\dot{y}(t)) = 0
\end{align}\\]

We can solve these equations as follows. Specifically, let's study solutions \\(\gamma\\) to the geodesic equations with unit speed \\(\|\dot{\gamma}(t)\| = 1\\). First observe that by the first equation
\\[
    y^2\frac{d}{d t}\left(y^{-2}\dot{x}(t)\right)
    = \ddot{x}(t) - \frac{2}{y(t)}\dot{x}(t)\dot{y}(t) = 0.
\\]
By \\(y(t) \neq 0\\) we must have \\(\frac{d}{d t}y^{-2}\dot{x}(t) = 0\\). Therefore we have \\(\dot{x}(t) = cy^2\\) for some constant \\(c\\). We could plug this into the second equation; however, equivalent information is encoded into our assumption that \\(\gamma\\) has unit speed:
\\[\begin{align}
    y^{-2}(\dot{x}(t)+\dot{y}(t)) \implies \dot{y}(t) = y\sqrt{1-(cy)^2}
\end{align}\\]
This allows for a simpler solution for \\(y(t)\\) through separation of variables /\*TODO\*/.

For \\(c = 0\\), this yields \\(y = y_0e^t\\) and \\(x = x_0\\). That is, vertical lines are geodesics.

For \\(c \neq 0\\), this yields
\\[
    y(t) = \frac{1}{c \cosh(t+t_0)} \implies x(t) = \frac{1}{c}\tanh(t+t_0)+a.
\\]
To visualize this, oberserve 
\\((x-a)^2+y^2 = \left(\frac{1}{c}\right)^2\\) and so half circles centered on the boundary \\(y = 0\\) are geodesics.

/\*cite iva\*/