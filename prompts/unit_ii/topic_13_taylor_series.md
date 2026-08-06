# Prompt — Topic 13: Power Series Expansions — Taylor's Series

**Unit:** II — Complex Variable: Integration  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 13: **Power Series Expansions: Taylor's Series** in complex analysis. Students know ordinary Taylor series from calculus; show how the complex version is both familiar and more powerful.

Use the same LaTeX framework and teaching style as earlier prompts.

Set:
- `\lhead{Topic 13: Taylor Series}`
- `\rhead{Unit II — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: In real calculus, a Taylor series is a useful approximation. In complex analysis, something remarkable happens: if a function is analytic, it is not just approximately equal to a power series near a point — it actually becomes that power series.

---

## REQUIRED SECTIONS

### 1. From Real Taylor Series to Complex Taylor Series
Bridge from familiar real-variable expansion.

### 2. Statement of Taylor Series for Analytic Functions
Present:
`f(z)=\sum_{n=0}^{\infty} \frac{f^{(n)}(z_0)}{n!}(z-z_0)^n`
Explain center and radius of convergence.

### 3. Maclaurin Series as Special Case
Explain the case `z_0=0`.

### 4. Radius of Convergence and Analytic Region
Explain that convergence extends up to nearest singularity. Use diagrams.

### 5. Standard Expansions
Include `e^z`, `\sin z`, `\cos z`, `1/(1-z)`, `\log(1+z)` where appropriate with convergence conditions.

### 6. Worked Examples
At least 8 examples including:
- `e^z`
- `\sin z`
- `1/(1-z)`
- expansion about nonzero center
- deriving coefficients using CIF derivative formula
Each example ends with learnbox.

### 7. Radius-of-Convergence Visual (MANDATORY UPGRADE)
Include a diagram of center point and nearest singularity determining convergence circle.

### 8. Excel Example (MANDATORY)
Show partial sums for a Taylor series and compare exact vs approximate values.

### 9. Python Example (MANDATORY)
Use Python to compute partial sums and plot approximation quality.

### 10. Viva Questions (8)
### 11. Descriptive Questions (5)
### 12. Practice Problems (6)
### 13. MCQs (5)
### 14. Common Mistakes
Include wrong center, ignoring convergence region, incorrect factorial terms, mixing Taylor with Laurent series.

### 15. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Taylor series formula included
- [ ] Maclaurin case included
- [ ] Radius of convergence explained
- [ ] At least 8 worked examples
- [ ] Convergence-circle diagram included
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
