# Prompt — Topic 07: Finding Harmonic Conjugate

**Unit:** I — Complex Variable: Differentiation  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 07: **Finding Harmonic Conjugate**. This should be highly procedural and example-rich, because students usually struggle with the integration steps and hidden constants/functions.

Use the same LaTeX framework and pedagogy as the previous topics.

Set fancyhdr:
- `\lhead{Topic 07: Harmonic Conjugate}`
- `\rhead{Unit I — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: Suppose someone gives you only the real part of an analytic function. Can you recover the missing imaginary part? Surprisingly, yes — if the given function is harmonic. The missing partner is called the harmonic conjugate.

---

## REQUIRED SECTIONS

### 1. Why Harmonic Conjugates Matter
Explain the goal: building analytic functions from one known real-valued part.

### 2. Definition
Define harmonic conjugate and relationship to `f(z)=u+iv`.

### 3. Method Using C-R Equations
Give the step-by-step procedure:
- Compute `u_x` and `u_y`
- Use `v_y=u_x`, `v_x=-u_y`
- Integrate carefully
- Introduce unknown function/constant where needed
- Compare and determine missing term

### 4. Alternative Starting from `v`
Show how to proceed if imaginary part is given instead.

### 5. Uniqueness Up to an Additive Constant
Explain clearly.

### 6. Worked Examples
At least 8 examples including:
- `u=x^2-y^2`
- `u=e^x\cos y`
- `u=\frac{x}{x^2+y^2}`
- given `v` instead of `u`
- one example that first checks harmonicity before proceeding
Every example ends with learnbox.

### 7. Procedure Summary Table (MANDATORY UPGRADE)
A compact table: Step | What to do | Why it is needed.

### 8. Excel Example (MANDATORY)
Use spreadsheet columns to compute partial derivatives numerically and infer consistency relations.

### 9. Python Example (MANDATORY)
Use sympy to compute partial derivatives and reconstruct a harmonic conjugate symbolically.

### 10. Viva Questions (8)
### 11. Descriptive Questions (5)
### 12. Practice Problems (6)
### 13. MCQs (5)
### 14. Common Mistakes
Include forgetting the arbitrary constant, missing function-of-one-variable during integration, sign errors in C-R equations, and proceeding without checking harmonicity.

### 15. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Clear step-by-step method included
- [ ] At least 8 worked examples
- [ ] Example starting from v included
- [ ] Uniqueness up to constant explained
- [ ] Procedure summary table included
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
