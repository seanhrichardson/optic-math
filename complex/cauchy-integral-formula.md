---
layout: page
title: Cauchy Integral Formula
---

## Cauchy Integral Formula

An important property of a holomorphic function \\(f(z)\\) is the component functions \\(u\\) and \\(v\\) are *harmonic* where \\(f(x+iy) = u(x+iy) + iv(x+iy)\\). That is, \\(\Delta u = \Delta v = 0\\) where \\(\Delta = \frac{\partial^2}{\partial x^2} + \frac{\partial^2}{\partial y^2}\\) is the Laplacian. 

**Exercise.** Use the Cauchy-Riemann equations to verify the component functions \\(u\\) and \\(v\\) are harmonic.

**Solution.** /\*hide this\*/ 
\\[
    \frac{\partial^2 u}{\partial x^2} 
    = \frac{\partial }{\partial x} \left( \frac{\partial v}{\partial y} \right) 
    = \frac{\partial }{\partial y} \left( \frac{\partial v}{\partial x} \right) 
    = \frac{\partial }{\partial y}\left( -\frac{\partial u}{\partial y} \right)
    = -\frac{\partial^2 u}{\partial y^2}
\\]
/\*todo do \\(v\\)\*/

Many physical phenomenon are modeled with harmonic functions, so these functions are well studied and well understood. Importantly, these functions satisfy the *mean value property*: the average value of a harmonic function over a circle is always the value of the function at the center of the circle. Because the components of holomorphic functions are harmonic, holomorphic functions also satisfy the mean value property. This property can be nicely rephrased and proved using only complex analysis -- without appealing to the general mean value property of harmonic functions. The result is the *Cauchy integral formula* and the first step is to rewrite the average value of a complex function over a circle of radius \\(1\\) centered at \\(z\\) as a complex contour integral as follows.
\\[
    \frac{1}{2\pi}\int_{\theta = 0}^{2\pi} f(z + e^{i\theta})d\theta = \frac{1}{2\pi i} \int\_{\gamma} \frac{f(\zeta)}{\zeta - z} d \zeta
\\]
where we made the change of variables \\(\zeta = z + e^{i\theta}\\) and the curve \\(\gamma\\) is the circle of radius \\(1\\) centered at \\(z\\). /\*briefly explain the following CIF is not surprising\*/

/\*state CIF\*/

/\*prove state CIF\*/