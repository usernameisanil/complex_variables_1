# Unit I — Complex Variable: Differentiation

**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  

---

## Overview

Unit I introduces the theory of functions of a complex variable, extending calculus concepts (limits, continuity, differentiation) to the complex plane. The central focus is on **analytic functions** — the class of complex functions that are differentiable in a region — characterized by the **Cauchy-Riemann equations**. The unit concludes with harmonic functions and practical methods for constructing analytic functions.

---

## Topic List (in teaching order)

| Topic No. | Topic Name | Prompt File |
|-----------|-----------|-------------|
| 01 | Introduction to Functions of Complex Variable | `prompts/unit_i/topic_01_intro_functions_complex_variable.md` |
| 02 | Concept of Limit & Continuity | `prompts/unit_i/topic_02_limit_continuity.md` |
| 03 | Differentiation | `prompts/unit_i/topic_03_differentiation.md` |
| 04 | Cauchy-Riemann Equations | `prompts/unit_i/topic_04_cauchy_riemann_equations.md` |
| 05 | Analytic Functions | `prompts/unit_i/topic_05_analytic_functions.md` |
| 06 | Harmonic Functions | `prompts/unit_i/topic_06_harmonic_functions.md` |
| 07 | Finding Harmonic Conjugate | `prompts/unit_i/topic_07_harmonic_conjugate.md` |
| 08 | Construction of Analytic Function by Milne Thomson Method | `prompts/unit_i/topic_08_milne_thomson_method.md` |

---

## Topic Descriptions

### Topic 01 — Introduction to Functions of Complex Variable

Builds the foundation for complex analysis by extending real number concepts to the complex plane. Covers:
- **Complex number recap:** z = x + iy, modulus |z|, argument arg(z), complex conjugate z̄
- **The complex plane (Argand diagram):** Cartesian and polar forms
- **Functions of a complex variable:** w = f(z) = u(x,y) + iv(x,y) where u, v are real-valued functions
- **Real and imaginary parts of complex functions:** extracting u(x,y) and v(x,y)
- **Examples:** f(z) = z², f(z) = eᶻ, f(z) = sin z expanded into real and imaginary parts
- **Mappings:** Concept of f(z) as a mapping from z-plane to w-plane

---

### Topic 02 — Concept of Limit & Continuity

Extends the ε-δ definitions of limit and continuity to complex functions. Covers:
- **Limit of f(z) as z → z₀:** The limit must be the same regardless of the path of approach
- **Non-existence of limits:** How approaching along different paths can yield different values
- **Continuity of f(z) at z₀:** lim f(z) = f(z₀)
- **Properties of continuous complex functions**
- **Examples demonstrating path-dependence** and why it matters in complex analysis

---

### Topic 03 — Differentiation

Defines the derivative of a complex function and explores its implications. Covers:
- **Derivative of f(z):** f'(z) = lim[Δz→0] [f(z+Δz) − f(z)] / Δz
- **Path independence requirement** for differentiability in the complex plane
- **Rules of differentiation:** Sum, product, quotient, chain rules (same form as real calculus)
- **Examples:** Differentiating polynomials, rational functions, and elementary complex functions
- **Contrast with real differentiability:** A function can be real-differentiable but not complex-differentiable

---

### Topic 04 — Cauchy-Riemann Equations

Derives and applies the fundamental necessary conditions for complex differentiability. Covers:
- **Derivation of C-R equations** by taking limits along real and imaginary axes:
  - ∂u/∂x = ∂v/∂y and ∂u/∂y = −∂v/∂x
- **C-R equations as necessary conditions** for differentiability
- **Sufficient conditions** for analyticity: C-R equations + continuity of partial derivatives
- **C-R equations in polar form:** ∂u/∂r = (1/r)∂v/∂θ, ∂v/∂r = −(1/r)∂u/∂θ
- **Worked examples:** Checking whether given functions satisfy C-R equations
- **Formula for f'(z):** f'(z) = ∂u/∂x + i∂v/∂x = ∂v/∂y − i∂u/∂y

---

### Topic 05 — Analytic Functions

Defines and explores the most important class of complex functions. Covers:
- **Definition:** f(z) is analytic at z₀ if it is differentiable at z₀ and in a neighbourhood of z₀
- **Entire functions:** Analytic everywhere (e.g., polynomials, eᶻ, sin z)
- **Singular points:** Points where f(z) fails to be analytic
- **Properties of analytic functions:** Sums, products, quotients, compositions
- **Examples and non-examples** with justification using C-R equations
- **Significance:** Analytic functions have extraordinary properties — they are infinitely differentiable and equal their Taylor series

---

### Topic 06 — Harmonic Functions

Connects analytic functions to solutions of Laplace's equation. Covers:
- **Definition:** A real-valued function φ(x,y) is harmonic if ∂²φ/∂x² + ∂²φ/∂y² = 0 (Laplace's equation)
- **Theorem:** If f(z) = u + iv is analytic, then both u and v are harmonic
- **Proof sketch:** Applying C-R equations to show u and v satisfy Laplace's equation
- **Applications:** Harmonic functions model steady-state heat distribution, electrostatics, fluid flow
- **Examples:** Verifying that u = x² − y², u = eˣ cos y are harmonic

---

### Topic 07 — Finding Harmonic Conjugate

Given one harmonic function, constructs its harmonic partner. Covers:
- **Definition:** If u is harmonic, then v is its harmonic conjugate if u + iv is analytic
- **Method using C-R equations:**
  - From ∂v/∂y = ∂u/∂x → integrate w.r.t. y to get v (with function of x)
  - From ∂v/∂x = −∂u/∂y → determine the function of x
- **Complete worked examples:** Given u = x² − y², find v; given u = eˣ cos y, find v
- **Uniqueness:** The harmonic conjugate is unique up to an additive constant
- **Constructing f(z):** Once v is found, write f(z) = u + iv and express in terms of z

---

### Topic 08 — Construction of Analytic Function by Milne Thomson Method

Provides an elegant direct method to construct analytic functions. Covers:
- **Milne Thomson method:** Constructing f(z) directly without finding v separately
- **Given u(x,y):** f(z) = ∫[φ₁(z,0) − iφ₂(z,0)] dz where φ₁ = ∂u/∂x, φ₂ = ∂u/∂y, substitute x=z, y=0
- **Given v(x,y):** f(z) = ∫[ψ₂(z,0) + iψ₁(z,0)] dz where ψ₁ = ∂v/∂x, ψ₂ = ∂v/∂y
- **Worked examples:** Finding f(z) given u or v
- **Advantage:** Bypasses the two-step C-R integration process
- **Verification:** Confirming results match the harmonic conjugate method

---

## Syllabus Coverage Map

| Syllabus Item | Covered In |
|---|---|
| Introduction to functions of complex variable | Topic 01 |
| Concept of Limit & continuity | Topic 02 |
| Differentiation | Topic 03 |
| Cauchy-Riemann equations | Topic 04 |
| Analytic functions | Topic 05 |
| Harmonic functions | Topic 06 |
| Finding harmonic conjugate | Topic 07 |
| Construction of analytic function by Milne Thomson method | Topic 08 |

---

## Prerequisites Needed

- Complex number arithmetic (modulus, argument, polar form)
- Real calculus: limits, continuity, partial derivatives
- Basic concept of mappings and functions
