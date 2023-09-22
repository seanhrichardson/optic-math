---
layout: page
title: Special Relativity
---

/\*maybe use YOUR coordinates and MY coordinates\*/

/\*avoid using coordinate notation (...). Instead, use \\(v^i\partial_i\\)\*/

## Special Relativity

/\*start with just \\(\mathbb{R}^{1+1}\\)... more intuiticve and allows for visuals.\*/

/\*briefly mention phenomenon of special relativity here\*/

#### Spacetime
/\*explain basic idea of spacetime, this will be centered around interactive visuals...\*/

/\*mention units are taken so speed of light is 1 up here?\*/

/\*list some implicit assumptions about inertial observers up here?\*/


#### Axioms

Suppose you are an inertial observer using coordinates \\((t,x,y,z)\\).

Many other coordinates \\((\tilde{t},\tilde{x},\tilde{y},\tilde{z})\\) are possible.

We wish to understand what other coorinate systems \\((\tilde{t},\tilde{x},\tilde{y},\tilde{z})\\) are possible.

Any other coordinate systems must obey some axioms:
1. All inertial observers measure the same speed of light \\(c\\).
2. If we observe an inertial observer moving at speed \\(\|v\|\\) relative to us, then they observe us moving at the same speed \\(\|v\|\\) relative to them.
3. The change of coordinate map between inertial observers is linear. /\*justify? ... this will be ditched in GR ... maybe make this linearization instead?\*/  /\*also add vector space axiom?\*/ /\*maybe just use linearization of manifold? maybe just say this is a linear approximation?\*/

#### Invariance of the Interval

Let's use these axioms to make some deductions about what coordinate systems are possible /\*reframe: want an invariant between coordinate systems...\*/, beginning by using the univsersality of the speed of light. Indeed, by axiom (1), according to your coordinates \\((t,x,y,z)\\), you will measure light in the following set (remember we chose units so that the speed of light \\(c\\) is \\(1\\)).
\\[
    Z = \left\\{(\Delta t,\Delta x, \Delta y, \Delta z) : \frac{\Delta x^2 + \Delta y^2 + \Delta z^2}{\Delta t^2} = c = 1 \right\\}.
\\]
We can rewrite this as the zero set 
\\[Z = \\{(\Delta t,\Delta x, \Delta y, \Delta z) : -\Delta t^2 + \Delta x^2 + \Delta y^2 + \Delta z^2 = 0\\}.\\]

By the same reasoning, any inertial observer using coordinates \\((\tilde{t},\tilde{x},\tilde{y},\tilde{z})\\) will measure light in the zero set 
\\[\tilde{Z} = \\{(\Delta \tilde{t},\Delta \tilde{x}, \Delta \tilde{y}, \Delta \tilde{z}) : - \Delta \tilde{t}^2 + \Delta \tilde{x}^2 + \Delta \tilde{y}^2 + \Delta \tilde{z}^2 = 0\\}.\\]

The sets \\(Z\\) and \\(\tilde{Z}\\) both describe the same region of the vector space that light will be observered, they were simply defined using different coordinates; that is, we have the set equality \\(\tilde{Z} = Z\\), which is a substantial restriction on the coordinates \\((\tilde{t},\tilde{x},\tilde{y},\tilde{z})\\). A convenient way to rewrite this findings is by defining a function \\(m: \mathbb{R}^{3+1} \times \mathbb{R}^{3+1} \to \mathbb{R}\\) in our coordinates \\((t,x,y,z)\\) as
\\[
    m((t\_1,x\_1,y\_1,z\_1),(t\_2,x\_2,y\_2,z\_2)) = -t\_1t\_2 + x\_1x\_2 + y\_1y\_2 + z\_1z\_2,
\\]
and defining a function \\(\tilde{m}: \mathbb{R}^{3+1} \times \mathbb{R}^{3+1} \to \mathbb{R}\\) in the other inertial observer's coordinates \\((\tilde{t},\tilde{x},\tilde{y},\tilde{z})\\) as
\\[
    \tilde{m}((\tilde{t}\_1,\tilde{x}\_1,\tilde{y}\_1,\tilde{z}\_1),(\tilde{t}\_2,\tilde{x}\_2,\tilde{y}\_2,\tilde{z}\_2)) = -\tilde{t}\_1\tilde{t}\_2 + \tilde{x}\_1\tilde{x}\_2 + \tilde{y}\_1\tilde{y}\_2 + \tilde{z}\_1\tilde{z}\_2.
\\]
Then our previous result can be re-written as
\\[
    \\{v: m(v,v) = 0\\} = \\{\tilde{v}: \tilde{m}(\tilde{v}, \tilde{v}) = 0\\}.
\\]
In other words, the zero sets of \\(m(v,v)\\) and \\(\tilde{m}(\tilde{v},\tilde{v})\\) are identical. Rewritting our findings in this way is helpful because we can apply the result of the following exercise.

**Exercise.**
/\*TODO: bilinear forms with same zeroes will be scalar multiples.\*/

**Solution.**
/\*TODO.\*/

By the above exercise, we conclude that there is some constant \\(\alpha\\) so that \\(m(v,v) = \alpha \tilde{m}(Lv, Lv)\\) for all \\(v\\). We will show that \\(\alpha = 1\\) using axiom (2). Indeed, consider the vectors \\(\partial_t\\) and \\(\partial_{\tilde{t}}\\). In our coordinates \\((t,x,y,z)\\) we can measure the speed \\(|v|\\) between us and the other inertial observer \\(\partial_t = (t_1,x_1,y_1,z_1)\\) by 
\\[\|v\|^2 = \frac{x_1^2+y_1^2+z_1^2}{t_1^2}\\]

??????????? actually this might not work ???????????

/\*OLD STUFF BELOW\*/
#### Lorentz Transformations
/\*define Lorentz transformations as all coordinate transformations.\*/

/\*\*/

#### Time Dilation and Length Contraction

#### Minkowski Metric
In this section, we give space-time a metric \\(m\\) that accurately captures the behavior of physics, the *Minkowski metric*. This will allow us to apply all the tools from Riemannian geometry to study relativity.

The laws of physics remain the same regarldess of how fast an inertial observer is moving, so the most important property of such a metric \\(m\\) is that *all inertial observers must observe the same metric*. In other words, the metric should be invariant under Lorentz transformations.

/\*Note to self: Geometry of a sphere stays the same under rotations, etc. Geometry (i.e. laws of physics) stay the same under Lorentz transformations.\*/

In fact, there is only one metric (up to scaling) that is invariant under Lorentz transformations, the *Minkowski metric*.

**Def.** The *Minkowski metric* is given by
\\[
    m = dx^2-dt^2
\\]

/\*note somewhere not a Riemannian metric, but rather a pseudo-riemannian metric.\*/

/\*Below reasons why the Minkowski metric is a good choice and the only choice.\*/

**Exercise.** Show that the Minkowski metric is invariant under Lorentz transformations.

**Solution.** TODO

**Exercise.** Show that any symmetric, bilinear map \\(m: \mathbb{R} \times \mathbb{R} \to \mathbb{R}\\) that is invariant under Lorentz transformations and satisfies \\(m(\partial_x, \partial_x) = 1\\) needs to be the Minkowsi metric.

**Solution.** TODO

**Exercise.** Show that all isometries of space-time \\(\mathbb{R} \times \mathbb{R}\\) under the Minkowski metric are Lorentz transformations.

**Solution.** TODO

#### Using the Minkowski Metric
In addition to invariance under Lorentz transformations, the Minkowski metric is useful in that we can use it to compute relative velocities between observers, the time that passes on each observers clock, and /\*time dilation, length contraction?\*/

Given two inertial observers \\(\partial_t\\) and \\(\partial_{\tilde{t}}\\), the relative velocity \\(v\\) between them is given by
\\[
    v = \sqrt{1- \frac{1}{m(\partial_t, \partial_{\tilde{t}})^2}}.
\\]
**Exercise.** Prove the above formula.

**Solution.**  /\*TODO... use Lorentz transformation.\*/

/\*Proper time\*/
\\[
    \tau = \int_{a}^{b}\sqrt{-m(\dot{\gamma}, \dot{\gamma})}ds
\\]



Recall that 

/\*motivation below... optional?\*/

#### Geodesics in Minkowski space-time

/\*Solve geodesic equations\*/

/\*Inertial observers are geodesic paths \\(\gamma\\) s.t \\(m(\dot{\gamma}, \dot{\gamma}) = -1\\)... maybe make this point earlier?\*/

/\*Jumping point into GR... observers in free-fall should also be inertial (motivate this), so the curvature should behave such that \*/

#### Apendix: Invariance of Minkowski Form Argument

**Scalar Multiple.**

Recall that in our coordinates, the symmetric bilinear form \\(m: V \times V \to \mathbb{R}\\) defined to be, for \\(w = w^t\partial_t + w^i \partial_i\\), given by
\\[m(u,v) = -u^tv^t + u^1v^1+u^2v^2+u^3v^3.\\]
We defined another bilinear form \\(\tilde{m}: V \times V \to \mathbb{R}\\) in other coordinates. We know \\(\tilde{m}\\) is symmetric, and \\(\tilde{m}(v,v) = 0\\) exactly when \\(m(v,v) = 0\\). In our coordinates, separating the time and the space coordinates, we know \\(\tilde{m}\\) is of the form
\\[\widetilde{m}(u,v) = u^tv^t\widetilde{m}\_{t,t} + 2u^tv^i\widetilde{m}\_{t,i} + u^iv^j\widetilde{m}\_{i,j}\\]
for unknown coefficients \\(\widetilde{m}\_{\alpha,\beta}\\) with \\(\alpha, \beta \in \\{t,1,2,3\\}\\). We now strategically evaluate \\(\widetilde{m}\\) at particular vectors to find these coefficients.

In your coordinates, consider the vectors \\(w = \partial_t + \partial_1\\) and \\(w' = \partial_t - \partial_1\\) noting \\(m(w,w) = 0\\) and \\(m(w',w')\\). Hence \\(\widetilde{m}(w,w) = 0\\) and \\(\widetilde{m}(w',w') = 0\\). Therefore,
\\[
    0 = \widetilde{m}(w',w') - \widetilde{m}(w,w) = \cdots = 4\widetilde{m}\_{t,1}.
\\]
Thus \\(\widetilde{m}\_{t,1} = 0\\) and by the same argument \\(\widetilde{m}\_{t,i} = 0\\) for all \\(i\\), yielding the updated expression
\\[
    \widetilde{m}(u,v) = u^tv^t\widetilde{m}\_{t,t} + u^iv^j\widetilde{m}\_{i,j}.
\\]
Next, define new vectors \\(w = \partial_t + \frac{1}{\sqrt{2}}(\partial_1 + \partial_2)\\) and \\(w' = \partial_t + \frac{1}{\sqrt{2}}(\partial_1 - \partial_2)\\). Note again we have \\(m(w,w) = 0\\) and \\(m(w',w')\\), thus \\(\widetilde{m}(w,w) = 0\\) and \\(\widetilde{m}(w',w') = 0\\). Therefore, we can conclude
\\[
    0 = \widetilde{m}(w,w) = \widetilde{m}(w',w') = \cdots = \widetilde{m}_{1,2}
\\]
Therefore \\(\widetilde{m}\_{1,2} = 0\\) and by the same argument, \\(\widetilde{m}\_{i,j} = 0\\) for all \\(i \neq j\\) and so we have the updated expression
\\[
    \widetilde{m}(u,v) = u^tv^t\widetilde{m}\_{t,t} + u^1v^1\widetilde{m}\_{1,1}+u^2v^2\widetilde{m}\_{2,2}+u^3v^3\widetilde{m}\_{3,3}.
\\]
Finally, define \\(w = \partial_t + \partial_i\\) for any \\(i\\). Again we have \\(m(w,w) = 0\\), thus \\(\widetilde{m}(w,w) = 0\\) and so
\\[
    0 = \widetilde{m}(w,w) = \widetilde{m}\_{t,t} + \widetilde{m}\_{i,i},
\\]
thus \\(\widetilde{m}\_{i,i} = -\widetilde{m}\_{t,t}\\) for all \\(i\\). Thus, taking \\(\alpha = -\widetilde{m}\_{t,t}\\), we conclude
\\[
    \widetilde{m}(u,v) = \alpha (-u^tv^t + u^1v^1+u^2v^2+u^3v^3) = \alpha \cdot m(u,v)
\\]

**Constant is 1.**

We have found that \\(\widetilde{m}(v,v) = \alpha m(v,v)\\) for some constant \\(\alpha\\). I now argue we in fact have \\(\alpha = 1\\). Indeed, by the principle of relativity, the constant \\(\alpha\\) can depend only on the relative speed between the coordinate systems \\((t,x,y,z)\\) and \\((\widetilde{t},\widetilde{x},\widetilde{y},\widetilde{z})\\). That is, if the observer \\((\widetilde{t},\widetilde{x},\widetilde{y},\widetilde{z})\\) carried out the same computation from their point of view, they should conclude \\(m(v,v) = \alpha \widetilde{m}(v,v)\\) for the same constant \\(\alpha\\). This can only be the case if \\(\alpha = 1\\).

/\*explain \\(m\\) is an invariant and define as inner product\*/

#### Lorentz Transformations

/\*explain: studying transormations between observer bases... showing these must be exactly the transformations that leave minkowski norm invariant\*/

Suppose you are an inertial observer and I am a separate inertial observer moving at speed \\(v\\) relative to you. Then, without loss of generality, you can choose a basis \\(\\{\partial_t, \partial_x, \partial_y, \partial_z\\}\\) so that you observe me moving in the positive \\(x\\) direction with velocity \\(v\\). That is,
\\[
    \partial\_{\widetilde{t}} = \frac{\partial\_t + v\partial\_x}{\sqrt{1-v^2}}.
\\]
I will also observe you going at velocity \\(v\\) relative to me and so without loss of generality, I can choose a basis \\(\\{\partial_\widetilde{t},\partial_\widetilde{x},\partial_\widetilde{y},\partial_\widetilde{z}\\}\\) so that I observe you moving in the negative \\(\widetilde{x}\\) direction with velocity \\(v.\\) That is,
\\[
    \partial\_{t} = \frac{\partial\_\widetilde{t} - v\partial\_\widetilde{x}}{\sqrt{1-v^2}}.
\\]
Combining the two equations above, we can conclude /\*TODO\*/
\\[
    \partial_{\widetilde{x}} = \frac{\partial_x + v\partial_t}{\sqrt{1-v^2}}.
\\]
It remains to find expressions for \\(\partial_{\widetilde{y}}\\) and \\(\partial_{\widetilde{z}}\\) in terms of \\(\\{\partial\_t, \partial\_x, \partial\_y, \partial\_z\\}\\). In other words, /\*this jump might need explanation or need to be avoided...\*/ given an arbitrary vector \\(v\\), written as \\(v = t\partial\_t + x\partial\_x + y\partial\_y + z\partial\_z\\) in your coordinates, and written as \\(v = \widetilde{t}\partial\_\widetilde{t} + \widetilde{x}\partial\_\widetilde{x} + \widetilde{y}\partial\_\widetilde{y} + \widetilde{z}\partial\_\widetilde{z}\\) in my coordinates, we would like to solve for \\(\\{\widetilde{t},\widetilde{x},\widetilde{y},\widetilde{z}\\}\\) in terms of \\(\\{t,x,y,z\\}\\). We already 
\\[
    .
\\]

Our goal now is to find the linear change of basis map \\(L: \mathbb{R}^{3+1} \to \mathbb{R}^{3+1}\\) so that if \\(v = t\partial_t + x\partial_x + y\partial_y + z\partial_z\\) represents the vector \\(v\\) in your basis, the map \\(L(t,x,y,z)\\) provides the coordinates \\((\widetilde{t},\widetilde{x},\widetilde{y},\widetilde{z})\\) for \\(v\\) in my coordinates.



\\[
    \partial_{\widetilde{x}} = \frac{\partial_x + v\partial_t}{\sqrt{1-v^2}}
\\]

/\*write out matrix form...\*/

Therefore, we can compute
\\[
    -\widetilde{t}
\\]

/\*use that \\(L\\) must leave minkowski form invariant to conclude \\(y^2+z^2 = \widetilde{y}^2+\widetilde{z}^2\\)\*/

/\*WLOG can rotate coordinates so that \\(y=\widetilde{y}\\) and \\(z=\widetilde{z}\\).\*/