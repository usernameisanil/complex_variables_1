# Prompt — Topic 17: Residues

**Unit:** II — Complex Variable: Integration  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 17: **Residues**. This should be highly procedural, formula-rich, and example-driven, because students must become fluent at extracting residues quickly and correctly.

Use the same LaTeX framework and style as earlier prompts.

Set:
- `\lhead{Topic 17: Residues}`
- `\rhead{Unit II — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: A Laurent series may contain infinitely many terms, but when contour integration enters the scene, one coefficient suddenly becomes the star of the show — the coefficient of `1/(z-z_0)`. That coefficient is called the residue, and it can determine the entire contour integral.

---

## REQUIRED SECTIONS

### 1. Definition of Residue
Define residue as the coefficient `a_{-1}` in the Laurent expansion about a singular point.

### 2. Why Residues Matter
Motivate their role in contour integration and later real-integral evaluation.

### 3. Residue Formulas
Include:
- coefficient method from Laurent series
- simple pole formula
- pole of order `m` formula
- `p(z)/q(z)` formula for simple poles

### 4. Choosing the Right Method
Explain how to decide which residue method to use.

### 5. Worked Examples
At least 9 examples including:
- simple pole
- double pole
- rational function with factorized denominator
- residue from Laurent expansion directly
- trigonometric/exponential-type example
Each example ends with learnbox.

### 6. Method Selection Table (MANDATORY UPGRADE)
Table: singularity type | best method | formula to use.

### 7. Excel Example (MANDATORY)
Use spreadsheet symbolic-style support or numerical sampling near a pole to illustrate coefficient behavior conceptually.

### 8. Python Example (MANDATORY)
Use sympy to compute residues for multiple sample functions.

### 9. Viva Questions (8)
### 10. Descriptive Questions (5)
### 11. Practice Problems (6)
### 12. MCQs (5)
### 13. Common Mistakes
Include forgetting to identify pole order first, sign errors after partial fractions, wrong derivative order in higher-order pole formula.

### 14. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Residue defined as coefficient of `a_{-1}`
- [ ] All main residue formulas included
- [ ] At least 9 worked examples
- [ ] Method-selection table included
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
