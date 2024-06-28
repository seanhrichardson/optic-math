---
layout: page
title: Holder Spaces
---

## Hölder spaces

#### Motivation via Arzelà-Ascoli

Often we are given a sequence of functions \\(u\_n\\) and wish to prove that this sequence converges uniformly /\*give examples to contextualize this claim... PDEs? \*/. If we are working on a compact subset \\(X \subset \mathbb{R}^n\\), the Arzelà-Ascoli theorem /\*link\*/ provides a convenient criteria for uniform convergence: pointwise boundedness and equicontinuity. Recall pointwise boundedness is the condition that for every \\(x \in X\\), the set \\(\\{u\_n(x)\\}\\) is bounded. Equicontinuity, which is generally harder to verify, is the condition that for every \\(\varepsilon > 0\\) and \\(x \in X\\) there is a \\(\delta > 0\\) such that \\(\\|x-y\\| < \delta\\) implies we have the bound \\(\|u\_n(x) - u\_n(y)\|\\) for all \\(u\_n\\). A convenient sufficient condition for equicontinuity is that there exists a fixed \\(C > 0\\) such that
\\[
    \|u(x) - u(y)\| \leq C \\|x-y\\| \tag{1} \label{eq:lipshitz}
\\]
for all \\(u \in \\{u\_n\\}\\). This immediately implies equicontinuity because for any \\(\varepsilon > 0\\) we can simply take \\(\\|x-y\\| < \varepsilon/C\\). However, an even weaker sufficient condition which is often easier to check is that for some fixed \\(\alpha \in (0,1]\\) there exists \\(C > 0\\) such that 
\\[
    \|u(x) - u(y)\| \leq C \\|x-y\\|^{\alpha} \tag{2} \label{eq:holder}
\\]
for all \\(u \in \\{u\_n\\}\\). In this case, we get equicontinuity by taking \\(\\|x-y\\| < \(\varepsilon/C\)^{1/\alpha}\\) for any given \\(\varepsilon > 0\\). If \\(u\\) satisfies \(\ref{eq:lipshitz}\), it is called "Lipshitz continuous" and if \\(u\\) satisfies \(\ref{eq:holder}\), it is called "\\(\alpha\\)-Hölder continuous". This terminology is due to the following exercise.

**Exercise.** Show that if \\(u: \mathbb{R}^n \to \mathbb{R}\\) satisfies either (1) or (2), it is a continuous function.

#### Hölder condition

/\*talk about Hölder condition and seminorm\*/

#### Holder spaces

/\*motivation... equicontinuity + pointwise boundedness\*/

**Def. (Hölder space).** /\*todo\*/

**Theorem.** /\*is a Banach space\*/

#### Compact embedding theorems

/\*recall motivation for Holder spaces... rephrase in terms of compact embeddings\*/

\\(C^{0, \alpha} \to C^0\\)

\\(C^{0, \alpha} \to C^{0, \beta}\\)

\\(C^{k, \alpha} \to C^{k}\\) /\*hopefully using earlier embedding\*/

\\(C^{k, \alpha} \to C^{k, \beta}\\) /\*hopefully using earlier embedding\*/