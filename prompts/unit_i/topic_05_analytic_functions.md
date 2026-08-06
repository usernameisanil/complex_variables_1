# Prompt — Topic 05: Analytic Functions

**Unit:** I — Complex Variable: Differentiation  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 05: **Analytic Functions**. This topic should build naturally from differentiability and Cauchy-Riemann equations.

Use the same LaTeX framework, tone, title-page format, and learning structure as the previous prompts.

Set fancyhdr:
- `\lhead{Topic 05: Analytic Functions}`
- `\rhead{Unit I — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: In ordinary calculus, differentiability at a point is already useful. In complex analysis, something far stronger happens: if a function is analytic, then it becomes one of the most well-behaved objects in all of mathematics.

---

## REQUIRED SECTIONS

### 1. From Differentiability to Analyticity
Clarify the difference between differentiable at a point and analytic in a neighborhood.

### 2. Definition of Analytic Function
Define analytic at a point, analytic in a region, and entire function.

### 3. Singular Points and Non-Analytic Behavior
Explain what it means for a point to be singular or non-analytic.

### 4. Properties of Analytic Functions
Discuss closure under addition, subtraction, multiplication, quotient (when denominator non-zero), and composition.

### 5. Relationship with C-R Equations
Explain how C-R + continuity of partial derivatives helps test analyticity.

### 6. Examples of Analytic and Non-Analytic Functions
Include examples like:
- polynomial functions
- `e^z`, `\sin z`, `\cos z`
- `\bar z`
- rational functions with excluded poles

### 7. Worked Examples
At least 7 examples with varying difficulty. Include determining where a function is analytic.
Each example ends with learnbox.

### 8. Visual Region-Based Interpretation (MANDATORY UPGRADE)
Include one diagram showing domains/regions where a function is analytic and where it is not, e.g. punctured plane for `1/z`.

### 9. Excel Example (MANDATORY)
Show how a spreadsheet can test C-R equations numerically at sampled points.

### 10. Python Example (MANDATORY)
Use sympy or numpy to analyze several functions and report candidate analytic regions.

### 11. Viva Questions (8)
### 12. Descriptive Questions (5)
### 13. Practice Problems (6)
### 14. MCQs (5)
### 15. Common Mistakes
Include differentiable-at-a-point vs analytic confusion, assuming C-R at one point is enough, ignoring denominator restrictions.

### 16. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Definition of analytic function clear
- [ ] Entire function explained
- [ ] Singular point idea included
- [ ] At least 7 worked examples
- [ ] Region/domain diagram included
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
