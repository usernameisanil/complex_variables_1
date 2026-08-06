# Prompt — Topic 02: Concept of Limit & Continuity

**Unit:** I — Complex Variable: Differentiation  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

You are an expert mathematics professor writing a **complete, compilable LaTeX (.tex) lecture note** for B.Tech engineering students on the topic **"Concept of Limit & Continuity"** in complex variables. This is Topic 02 of Unit I. Students know limits and continuity from single-variable calculus; your task is to help them see what changes when the variable becomes complex.

---

## LATEX SETUP REQUIREMENTS

Use the same preamble structure as Topic 01 with tcolorbox environments, fancyhdr, pgfplots, tikz, listings, and title page.
Set:
- `\lhead{Topic 02: Limit and Continuity}`
- `\rhead{Unit I — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK (MANDATORY)

Inside curiositybox: In real calculus, a point can be approached only from the left or the right. In complex analysis, a point can be approached from infinitely many directions. That single difference makes limits in the complex plane much stricter — and much more interesting.

---

## REQUIRED SECTIONS

### 1. Why Complex Limits Are Different
Compare real-variable limits with complex-variable limits. Emphasize infinitely many paths. Include a 2-column table: "Real-variable limit" vs "Complex-variable limit".

### 2. Formal Definition of Limit
Define `\lim_{z \to z_0} f(z) = l` using epsilon-delta language in an accessible way. Explain neighborhood of a point in the complex plane.

### 3. Path Dependence and Path Independence
Explain that the limit exists only if the same value is obtained along every possible path toward `z_0`.
Include at least 4 worked examples:
- A function whose limit exists
- A function whose limit fails because of different path values
- Approaching along `y=mx`
- Approaching along `y=x^2`

### 4. Theorems on Limits
State and explain standard theorems for sum, difference, product, quotient, scalar multiple. Include examples.

### 5. Continuity of Complex Functions
Define continuity at a point and in a region.
Explain:
- `f(z)` continuous at `z_0` if `\lim_{z\to z_0} f(z)=f(z_0)`
- continuity of polynomials
- continuity of rational functions except where denominator is zero

### 6. Geometric Interpretation
Explain what continuity means geometrically in the complex plane. Include one diagram showing approach to a point along different paths.

### 7. Worked Examples
At least 6 total worked examples, including:
- `f(z)=z^2`
- `f(z)=\bar z`
- `f(z)=\frac{x^2y}{x^4+y^2}`-type path-test example
- Rational function continuity at allowed points
Each ends with learnbox.

### 8. Excel Example (MANDATORY)
Show a spreadsheet setup for evaluating a function at points near `z_0` along different paths and comparing outputs numerically.

### 9. Python Example (MANDATORY)
Python script to evaluate a function near the origin along multiple paths and plot/print values to illustrate existence or failure of limit.

### 10. Viva Questions (8)
### 11. Descriptive Questions (5)
### 12. Practice Problems (6)
### 13. MCQs (5)
### 14. Common Mistakes
Include mistakes like checking only one path, confusing continuity with differentiability, and not handling denominator restrictions.

### 15. Quick Recap
6–8 bullets.

---

## MANDATORY QUALITY CHECKLIST

- [ ] Opening hook present
- [ ] At least 1 diagram for path approach
- [ ] At least 6 worked examples
- [ ] At least 1 Excel example
- [ ] At least 1 Python example
- [ ] Path-based nonexistence example included
- [ ] All four tcolorbox environments used
- [ ] `\end{document}` present
