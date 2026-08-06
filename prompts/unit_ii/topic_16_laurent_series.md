# Prompt — Topic 16: Laurent's Series

**Unit:** II — Complex Variable: Integration  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 16: **Laurent's Series**. Students should see Laurent series as a natural extension of Taylor series when singularities are present.

Use the same LaTeX framework and style as previous prompts.

Set:
- `\lhead{Topic 16: Laurent Series}`
- `\rhead{Unit II — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: Taylor series are perfect when a function is analytic at the center. But what if the function has a singularity there? Laurent series rescue the situation by allowing negative powers, and those negative powers reveal the exact nature of the singularity.

---

## REQUIRED SECTIONS

### 1. Why Taylor Series Is Not Enough
Use an example like `1/z` to motivate the need for negative powers.

### 2. Statement / Form of Laurent Series
Present:
`f(z)=\sum_{n=-\infty}^{\infty} a_n (z-z_0)^n`
Explain annular region of convergence.

### 3. Principal Part and Analytic Part
Define both clearly.

### 4. Connection with Singularity Classification
Explain how removable singularity / pole / essential singularity appear in the principal part.

### 5. Methods of Expansion
Show techniques:
- algebraic rewriting
- geometric-series expansion
- splitting into partial fractions
- choosing expansion based on region

### 6. Worked Examples
At least 8 examples including multiple regions for the same function, e.g. `1/[z(z-1)]`.
Each example ends with learnbox.

### 7. Region-Sensitive Expansion Table (MANDATORY UPGRADE)
Table: function | center | region | resulting series form.

### 8. Excel Example (MANDATORY)
Use spreadsheet partial sums to numerically illustrate approximation in an annulus.

### 9. Python Example (MANDATORY)
Use sympy to obtain series expansions and compare in different regions where possible.

### 10. Viva Questions (8)
### 11. Descriptive Questions (5)
### 12. Practice Problems (6)
### 13. MCQs (5)
### 14. Common Mistakes
Include expanding about wrong center, using wrong convergence region, not separating principal and analytic parts.

### 15. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Laurent form included
- [ ] Annular region explained
- [ ] Principal part defined
- [ ] At least 8 worked examples
- [ ] Multi-region example included
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
