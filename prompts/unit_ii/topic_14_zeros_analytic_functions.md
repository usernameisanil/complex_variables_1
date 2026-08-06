# Prompt — Topic 14: Zeros of Analytic Functions

**Unit:** II — Complex Variable: Integration  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 14: **Zeros of Analytic Functions**. Keep the treatment intuitive but mathematically correct, with clear linkage to Taylor series.

Use the same LaTeX framework and style as previous prompts.

Set:
- `\lhead{Topic 14: Zeros of Analytic Functions}`
- `\rhead{Unit II — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: A polynomial can have repeated roots like `(z-1)^3`. Analytic functions generalize this idea in a beautiful way: zeros are not just points where the function becomes zero, they also carry an order or multiplicity, and that order tells us a great deal about the local behavior of the function.

---

## REQUIRED SECTIONS

### 1. Definition of Zero
Define zero of analytic function and motivate with familiar polynomial examples.

### 2. Order / Multiplicity of a Zero
Explain simple zero, zero of order `m`, and the derivative test.

### 3. Taylor-Series Viewpoint
Show how `f(z)=(z-z_0)^m g(z)` with `g(z_0)\neq 0` emerges from Taylor expansion.

### 4. Isolated Nature of Zeros
Explain why zeros of a nontrivial analytic function are isolated.

### 5. Examples of Zeros in Standard Functions
Use polynomials, `\sin z`, `(z-i)^3`, etc.

### 6. Worked Examples
At least 7 examples including finding order of zeros, locating zeros, and using derivative conditions.
Each example ends with learnbox.

### 7. Multiplicity Test Table (MANDATORY UPGRADE)
Table: condition on derivatives | multiplicity conclusion.

### 8. Excel Example (MANDATORY)
Show numerical evaluation of a function near a zero to illustrate how higher-order zeros flatten behavior.

### 9. Python Example (MANDATORY)
Use symbolic/numeric computation to detect zeros and multiplicity for example functions.

### 10. Viva Questions (8)
### 11. Descriptive Questions (5)
### 12. Practice Problems (6)
### 13. MCQs (5)
### 14. Common Mistakes
Include assuming every zero is simple, forgetting to test derivatives in order, mixing zeros with singularities.

### 15. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Zero and multiplicity defined
- [ ] Taylor-series factor form included
- [ ] Isolated-zero idea explained
- [ ] At least 7 worked examples
- [ ] Multiplicity test table included
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
