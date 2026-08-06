# Prompt — Topic 03: Differentiation

**Unit:** I — Complex Variable: Differentiation  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 03: **Differentiation** in complex variables. Students know differentiation in real calculus; explain what is preserved and what becomes stricter in complex analysis.

Use the same LaTeX style, boxes, title-page structure, conversational tone, and pedagogical quality as Topic 01.

Set fancyhdr:
- `\lhead{Topic 03: Differentiation}`
- `\rhead{Unit I — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: In real calculus, a derivative checks one direction of change along the number line. In complex analysis, the increment can approach zero from infinitely many directions in the plane. So if a derivative exists, the function has passed a much tougher test.

---

## REQUIRED SECTIONS

### 1. Why Complex Differentiation Is Special
Explain the contrast with ordinary derivatives and why complex differentiability is more restrictive.

### 2. Definition of Derivative
Define:
`f'(z)=\lim_{\Delta z\to 0}\frac{f(z+\Delta z)-f(z)}{\Delta z}`
Explain the role of path independence in the increment `\Delta z`.

### 3. Differentiability vs Derivative at a Point
Explain meaning carefully. Discuss existence at a point and over a region.

### 4. Standard Differentiation Rules
Present sum, product, quotient, constant multiple, chain rule, with examples.

### 5. Differentiation of Standard Complex Functions
Cover:
- Polynomials
- Rational functions
- `e^z`
- `\sin z`, `\cos z`
- brief mention of logarithm branch issue

### 6. Why Path Independence Matters
Show derivation idea by taking `\Delta z` along real and imaginary directions. Prepare students for Cauchy-Riemann equations in next topic.

### 7. Worked Examples
At least 6 examples including:
- Derivative of `z^2`
- Derivative of `1/z`
- Show `\bar z` is not differentiable
- Piecewise or mixed-form example testing differentiability
Every example ends with learnbox.

### 8. Excel Example (MANDATORY)
Approximate derivative numerically using nearby values of `z` and compare along two paths.

### 9. Python Example (MANDATORY)
Numerically approximate the difference quotient for a differentiable function and a non-differentiable function, showing contrast.

### 10. Viva Questions (8)
### 11. Descriptive Questions (5)
### 12. Practice Problems (6)
### 13. MCQs (5)
### 14. Common Mistakes
Include mistakes like treating real differentiability as enough, ignoring direction of increment, and algebraic errors in complex quotient simplification.

### 15. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Opening hook present
- [ ] Derivative definition explained clearly
- [ ] At least 6 worked examples
- [ ] Includes non-differentiable example
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
