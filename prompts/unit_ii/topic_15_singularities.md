# Prompt — Topic 15: Singularities

**Unit:** II — Complex Variable: Integration  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 15: **Singularities**. This topic must be careful, classification-driven, and example-rich because it is foundational for Laurent series and residues.

Use the same LaTeX framework and style as previous prompts.

Set:
- `\lhead{Topic 15: Singularities}`
- `\rhead{Unit II — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: Analytic functions are beautifully smooth — until they suddenly fail to be analytic at certain points. Those exceptional points are singularities, and the way a function misbehaves there tells us almost everything we need for later contour-integration techniques.

---

## REQUIRED SECTIONS

### 1. What Is a Singularity?
Define singular point and isolated singularity.

### 2. Classification of Isolated Singularities
Explain:
- removable singularity
- pole of order `m`
- essential singularity
Use simple intuition and formal conditions.

### 3. Removable Singularities
Explain limit-based criterion and examples.

### 4. Poles
Define simple pole and higher-order poles. Connect to denominator zeros.

### 5. Essential Singularities
Explain infinite principal-part idea informally and use a classic example like `e^{1/z}`.

### 6. Classification via Algebraic Simplification and Series View
Explain how factor cancellation, denominator order, and later Laurent ideas help classify.

### 7. Worked Examples
At least 8 examples including:
- `(\sin z)/z`
- `1/(z-1)`
- `1/(z-2)^3`
- `e^{1/z}`
- rational function with removable singularity after cancellation
Every example ends with learnbox.

### 8. Classification Decision Table (MANDATORY UPGRADE)
Table: observed behavior | singularity type | quick test.

### 9. Excel Example (MANDATORY)
Sample function values near candidate singular points to illustrate blow-up, finite limit, or erratic behavior.

### 10. Python Example (MANDATORY)
Plot or tabulate behavior near singular points for several functions.

### 11. Viva Questions (8)
### 12. Descriptive Questions (5)
### 13. Practice Problems (6)
### 14. MCQs (5)
### 15. Common Mistakes
Include confusing zero with removable singularity, assuming every denominator zero gives simple pole, and calling `e^{1/z}` a pole.

### 16. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Isolated singularity defined
- [ ] All three types classified
- [ ] At least 8 worked examples
- [ ] Decision table included
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
