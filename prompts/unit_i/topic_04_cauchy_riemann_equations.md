# Prompt — Topic 04: Cauchy-Riemann Equations

**Unit:** I — Complex Variable: Differentiation  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 04: **Cauchy-Riemann Equations**. This topic is central to Unit I, so ensure strong conceptual clarity, careful derivation, and lots of checking examples.

Use the same LaTeX framework and teaching style as earlier topics.

Set fancyhdr:
- `\lhead{Topic 04: Cauchy-Riemann Equations}`
- `\rhead{Unit I — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: Here is the surprise of complex analysis: to be differentiable, a complex function cannot let its real and imaginary parts behave independently. They must satisfy two beautiful coupling equations. Those are the Cauchy-Riemann equations.

---

## REQUIRED SECTIONS

### 1. Why We Need C-R Equations
Connect to the previous topic's path-independence requirement.

### 2. Setting Up `f(z)=u(x,y)+iv(x,y)`
Explain role of `u` and `v`.

### 3. Derivation of C-R Equations
Derive by taking increment along real axis and imaginary axis separately.
State:
- `u_x = v_y`
- `u_y = -v_x`
Do the derivation step by step.

### 4. Interpretation of the Equations
Explain what they mean conceptually.

### 5. Necessary vs Sufficient Conditions
Explain clearly:
- If differentiable, C-R must hold.
- If C-R holds and first partial derivatives are continuous in a neighborhood, then differentiability follows.

### 6. Polar Form of C-R Equations
Include the polar form and explain when it is useful.

### 7. Formula for Derivative in Terms of Partial Derivatives
Show equivalent forms of `f'(z)`.

### 8. Worked Examples
At least 8 examples, including:
- `z^2`
- `e^z`
- `\bar z`
- `x^2+y^2 + i(2xy)`-style examples
- one example where C-R holds at a point but function is not analytic in neighborhood
Each example ends with learnbox.

### 9. Flowchart for Testing Analyticity (MANDATORY UPGRADE)
Provide a text-based or TikZ flowchart:
1. Write `u` and `v`
2. Find partial derivatives
3. Check C-R
4. Check continuity of partials
5. Conclude differentiable/analytic or not

### 10. Excel Example (MANDATORY)
Use spreadsheet columns to compute approximate partial derivatives of `u` and `v` numerically at selected points.

### 11. Python Example (MANDATORY)
Symbolic/numeric example using sympy to compute `u_x, u_y, v_x, v_y` and check C-R equations.

### 12. Viva Questions (8)
### 13. Descriptive Questions (5)
### 14. Practice Problems (6)
### 15. MCQs (5)
### 16. Common Mistakes
Include mistakes such as:
- checking C-R at only one point and declaring analytic everywhere
- forgetting continuity of partial derivatives
- incorrect sign in `u_y=-v_x`
- mixing `x,y` and `r,\theta`

### 17. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Full derivation included
- [ ] Necessary vs sufficient clearly separated
- [ ] Polar form included
- [ ] At least 8 worked examples
- [ ] Flowchart included
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
