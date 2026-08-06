# Prompt — Topic 12: Cauchy Integral Formula

**Unit:** II — Complex Variable: Integration  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 12: **Cauchy Integral Formula**. Present it as one of the most powerful tools in the course, with intuition, statement, derivative forms, and many examples.

Use the same LaTeX framework and pedagogical style as previous prompts.

Set:
- `\lhead{Topic 12: Cauchy Integral Formula}`
- `\rhead{Unit II — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: Usually, to know the value of a function at a point, we evaluate it directly at that point. Cauchy's Integral Formula says something astonishing: for analytic functions, the value at an interior point is completely determined by the values of the function all around a surrounding contour.

---

## REQUIRED SECTIONS

### 1. Why This Formula Is Extraordinary
Explain the idea of interior values being determined by boundary values.

### 2. Statement of Cauchy Integral Formula
State the formula clearly with assumptions.

### 3. Intuitive Interpretation
Explain in simple language what the formula means.

### 4. Derivative Forms
State the generalized formula for `f^{(n)}(z_0)`.
Explain why this implies analytic functions are infinitely differentiable.

### 5. Consequences
Mention analyticity strength, mean-value flavor, and evaluation of contour integrals.

### 6. Worked Examples
At least 8 examples, including:
- direct evaluation using unit circle
- higher derivative example
- rational integrand rewritten in CIF form
- examples with center not at origin
Each example ends with learnbox.

### 7. Formula Recognition Table (MANDATORY UPGRADE)
Table: integrand form | identify `f(z)` | identify `z_0` | order used.

### 8. Excel Example (MANDATORY)
Numerically sample points on a circle and illustrate how boundary values contribute to interior point evaluation.

### 9. Python Example (MANDATORY)
Approximate the integral formula numerically for a simple analytic function on a circle.

### 10. Viva Questions (8)
### 11. Descriptive Questions (5)
### 12. Practice Problems (6)
### 13. MCQs (5)
### 14. Common Mistakes
Include wrong identification of `z_0`, forgetting contour must enclose point, mishandling derivative order, missing `2\pi i` factor.

### 15. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] CIF statement included
- [ ] Derivative formula included
- [ ] At least 8 worked examples
- [ ] Recognition table included
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
