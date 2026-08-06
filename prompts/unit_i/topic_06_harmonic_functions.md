# Prompt — Topic 06: Harmonic Functions

**Unit:** I — Complex Variable: Differentiation  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 06: **Harmonic Functions**. Students should understand both the PDE viewpoint and the connection to analytic functions.

Use the same LaTeX framework and style as previous prompts.

Set fancyhdr:
- `\lhead{Topic 06: Harmonic Functions}`
- `\rhead{Unit I — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: A thin metal plate reaches a steady temperature distribution. No heat is building up anywhere, and none is disappearing mysteriously. The temperature function that describes this balance often satisfies Laplace's equation. In complex analysis, such functions appear naturally as the real and imaginary parts of analytic functions.

---

## REQUIRED SECTIONS

### 1. Motivation from Physics and Engineering
Connect harmonic functions to heat flow, electrostatics, and fluid flow.

### 2. Definition of Harmonic Function
Define `u(x,y)` harmonic if `u_{xx}+u_{yy}=0`.
Explain Laplace's equation.

### 3. Connection with Analytic Functions
State and explain that if `f(z)=u+iv` is analytic, then `u` and `v` are harmonic.
Provide proof using C-R equations.

### 4. Geometric/Physical Interpretation
Explain balance, no local source/sink idea, smooth potential-like behavior.

### 5. Testing Whether a Function Is Harmonic
Step-by-step method.

### 6. Worked Examples
At least 7 examples, including:
- `u=x^2-y^2`
- `u=e^x\cos y`
- one non-harmonic example
- one example tied back to an analytic function
Every example ends with learnbox.

### 7. Contour/Surface Visualization (MANDATORY UPGRADE)
Include one pgfplots or tikz visualization of a harmonic function surface or contour map.

### 8. Excel Example (MANDATORY)
Show finite-difference style approximation of second partial derivatives on a grid.

### 9. Python Example (MANDATORY)
Use numpy/matplotlib to visualize a harmonic function as contour plot or surface plot.

### 10. Viva Questions (8)
### 11. Descriptive Questions (5)
### 12. Practice Problems (6)
### 13. MCQs (5)
### 14. Common Mistakes
Include wrong second derivative computation, assuming every smooth function is harmonic, and confusing harmonic with analytic.

### 15. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Laplace equation defined
- [ ] Proof analytic => harmonic included
- [ ] At least 7 worked examples
- [ ] At least 1 contour/surface visualization
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
