# Unit II — Complex Variable: Integration

**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  

---

## Overview

Unit II extends integration to the complex plane. Starting from line integrals and contour integration, it develops the powerful theorems of Cauchy — the Integral Theorem and Integral Formula — then explores power series representations (Taylor and Laurent), classification of singularities, and the Residue Theorem with its application to evaluating definite integrals.

---

## Topic List (in teaching order)

| Topic No. | Topic Name | Prompt File |
|-----------|-----------|-------------|
| 09 | Line Integral | `prompts/unit_ii/topic_09_line_integral.md` |
| 10 | Contour Integration | `prompts/unit_ii/topic_10_contour_integration.md` |
| 11 | Cauchy's Integral Theorem (Simple Case) | `prompts/unit_ii/topic_11_cauchy_integral_theorem.md` |
| 12 | Cauchy Integral Formula | `prompts/unit_ii/topic_12_cauchy_integral_formula.md` |
| 13 | Power Series Expansions: Taylor's Series | `prompts/unit_ii/topic_13_taylor_series.md` |
| 14 | Zeros of Analytic Functions | `prompts/unit_ii/topic_14_zeros_analytic_functions.md` |
| 15 | Singularities | `prompts/unit_ii/topic_15_singularities.md` |
| 16 | Laurent's Series | `prompts/unit_ii/topic_16_laurent_series.md` |
| 17 | Residues | `prompts/unit_ii/topic_17_residues.md` |
| 18 | Cauchy Residue Theorem (Without Proof) | `prompts/unit_ii/topic_18_cauchy_residue_theorem.md` |
| 19 | Evaluation of Definite Integral Involving Sine and Cosine | `prompts/unit_ii/topic_19_definite_integrals_sine_cosine.md` |

---

## Topic Descriptions

### Topic 09 — Line Integral

Introduces integration of complex functions along curves in the complex plane. Covers:
- **Definition:** ∫_C f(z) dz where C is a curve (path) in the complex plane
- **Parametric representation:** z(t) = x(t) + iy(t), dz = (dx + i dy)
- **Computation:** ∫_C f(z) dz = ∫_a^b f(z(t)) z'(t) dt
- **Properties:** Linearity, reversal of path, splitting of path
- **ML inequality (estimation lemma):** |∫_C f(z) dz| ≤ M·L where M = max|f(z)|, L = length of C
- **Worked examples:** Line integrals along straight lines and circular arcs

---

### Topic 10 — Contour Integration

Formalises integration along closed curves and introduces key contour types. Covers:
- **Contour:** A piecewise smooth curve in the complex plane
- **Simple closed contour (Jordan curve):** A closed curve that does not cross itself
- **Positive orientation:** Counterclockwise traversal
- **Standard contours:** Circles, rectangles, semicircles
- **Relationship between contour integrals and path:** When the result depends/does not depend on the path
- **Worked examples:** Evaluating ∮_C dz/z around the unit circle

---

### Topic 11 — Cauchy's Integral Theorem (Simple Case)

States and applies the most fundamental theorem of complex integration. Covers:
- **Statement:** If f(z) is analytic in a simply connected domain D and C is any simple closed contour in D, then ∮_C f(z) dz = 0
- **Simply connected domain:** A region with no holes
- **Proof idea (Green's theorem approach):** Using C-R equations to reduce to zero
- **Deformation of contour principle:** The integral depends only on the topology, not the exact path
- **Corollary:** Path independence for analytic functions
- **Worked examples and counterexamples** (when the theorem fails — singularity inside C)

---

### Topic 12 — Cauchy Integral Formula

Derives the formula that expresses f(z₀) as a contour integral — one of the most powerful results in analysis. Covers:
- **Cauchy Integral Formula:** f(z₀) = (1/2πi) ∮_C f(z)/(z − z₀) dz
- **Generalized formula for derivatives:** f⁽ⁿ⁾(z₀) = (n!/2πi) ∮_C f(z)/(z − z₀)ⁿ⁺¹ dz
- **Implication:** Analytic functions are infinitely differentiable
- **Morera's Theorem** (converse of Cauchy's theorem)
- **Worked examples:** Evaluating contour integrals using the formula
- **Applications:** Computing integrals that would be intractable by direct methods

---

### Topic 13 — Power Series Expansions: Taylor's Series

Represents analytic functions as power series around a point. Covers:
- **Taylor's theorem for complex functions:** f(z) = Σ aₙ(z − z₀)ⁿ where aₙ = f⁽ⁿ⁾(z₀)/n!
- **Radius of convergence:** The largest circle within which the series converges
- **Maclaurin series** (Taylor series at z₀ = 0)
- **Standard expansions:** eᶻ, sin z, cos z, 1/(1−z), ln(1+z)
- **Uniqueness of Taylor series:** An analytic function has exactly one power series representation
- **Worked examples:** Finding Taylor series of given functions

---

### Topic 14 — Zeros of Analytic Functions

Classifies and analyses points where an analytic function vanishes. Covers:
- **Definition:** z₀ is a zero of f(z) if f(z₀) = 0
- **Order (multiplicity) of a zero:** z₀ is a zero of order m if f(z₀) = f'(z₀) = ... = f⁽ᵐ⁻¹⁾(z₀) = 0 but f⁽ᵐ⁾(z₀) ≠ 0
- **Isolated zeros:** Zeros of non-trivial analytic functions are isolated
- **Connection to Taylor series:** f(z) = (z − z₀)ᵐ g(z) where g(z₀) ≠ 0
- **Examples:** Zeros of sin z, (z² − 1), (z − i)³

---

### Topic 15 — Singularities

Classifies points where an analytic function fails to be analytic. Covers:
- **Isolated singularity:** z₀ where f is analytic in 0 < |z − z₀| < r but not at z₀ itself
- **Removable singularity:** lim f(z) exists as z → z₀; the Laurent series has no negative power terms
- **Pole of order m:** Laurent series has finite number of negative powers; (z − z₀)ᵐ f(z) → finite non-zero limit
- **Essential singularity:** Infinite negative power terms in Laurent series; e.g., e^(1/z) at z = 0
- **Behaviour near singularities:** Riemann's theorem (removable), poles, Picard's theorem (essential)
- **Worked examples:** Classifying singularities of given functions

---

### Topic 16 — Laurent's Series

Generalises Taylor series to functions with singularities. Covers:
- **Laurent's theorem:** f(z) = Σₙ₌₋∞^∞ aₙ(z − z₀)ⁿ valid in an annular region r < |z − z₀| < R
- **Principal part:** The sum of terms with negative powers
- **Analytic part:** The sum of terms with non-negative powers
- **Computing coefficients:** aₙ = (1/2πi) ∮_C f(z)/(z − z₀)ⁿ⁺¹ dz
- **Practical computation:** Using known series (geometric, exponential) to expand
- **Connection to singularity classification** via the principal part
- **Worked examples:** Expanding 1/[z(z−1)], e^(1/z), 1/(z²+1) in Laurent series

---

### Topic 17 — Residues

Defines and computes the key quantity used in the Residue Theorem. Covers:
- **Residue definition:** Res[f, z₀] = a₋₁ = coefficient of 1/(z − z₀) in the Laurent series
- **Residue at a simple pole:** Res[f, z₀] = lim[(z − z₀)f(z)] as z → z₀
- **Residue at a pole of order m:** Res[f, z₀] = (1/(m−1)!) lim d⁽ᵐ⁻¹⁾/dz⁽ᵐ⁻¹⁾ [(z−z₀)ᵐ f(z)]
- **Residue for f(z) = p(z)/q(z):** Res = p(z₀)/q'(z₀) when z₀ is a simple zero of q
- **Worked examples:** Computing residues of various rational and transcendental functions

---

### Topic 18 — Cauchy Residue Theorem (Without Proof)

States the theorem that transforms contour integrals into residue computations. Covers:
- **Statement:** ∮_C f(z) dz = 2πi × Σ Res[f, zₖ] for all poles zₖ inside C
- **Strategy for evaluating contour integrals:** Identify poles inside C, compute residues, sum and multiply by 2πi
- **Relationship to Cauchy Integral Formula** (special case)
- **Worked examples:** Evaluating ∮ f(z) dz for rational functions and mixed functions
- **Sign and orientation:** Positive (counterclockwise) orientation convention

---

### Topic 19 — Evaluation of Definite Integral Involving Sine and Cosine

Applies the Residue Theorem to evaluate real definite integrals. Covers:
- **Type I: ∫₀²π R(cos θ, sin θ) dθ**
  - Substitution: z = e^(iθ), cos θ = (z + 1/z)/2, sin θ = (z − 1/z)/2i, dθ = dz/(iz)
  - Reduces to a contour integral over the unit circle
- **Complete worked examples:** Step-by-step evaluation of standard integrals
- **Verification:** Confirming results against known values
- **Common pitfalls:** Ensuring all poles inside the unit circle are correctly identified

---

## Syllabus Coverage Map

| Syllabus Item | Covered In |
|---|---|
| Line integral | Topic 09 |
| Contour integration | Topic 10 |
| Cauchy's integral theorem (Simple Case) | Topic 11 |
| Cauchy Integral formula | Topic 12 |
| Power series expansions: Taylor's series | Topic 13 |
| Zeros of analytic functions | Topic 14 |
| Singularities | Topic 15 |
| Laurent's series | Topic 16 |
| Residues | Topic 17 |
| Cauchy Residue theorem (without proof) | Topic 18 |
| Evaluation of definite integral involving sine and cosine | Topic 19 |

---

## Prerequisites Needed

- Unit I material: Analytic functions, C-R equations
- Real integration and calculus
- Parametric curves and basic curve geometry
- Power series in real variables
