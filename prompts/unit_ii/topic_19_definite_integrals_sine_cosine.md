# Prompt — Topic 19: Evaluation of Definite Integral Involving Sine and Cosine

**Unit:** II — Complex Variable: Integration  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 19: **Evaluation of Definite Integral Involving Sine and Cosine** using complex-variable methods. This is the culmination of Unit II, so connect it clearly to contour integration, residues, and substitutions on the unit circle.

Use the same LaTeX framework and teaching style as previous prompts.

Set:
- `\lhead{Topic 19: Definite Integrals with Sine and Cosine}`
- `\rhead{Unit II — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: Some real integrals involving sine and cosine look unpleasant by ordinary trigonometric methods. Complex analysis offers a shortcut: wrap the interval around the unit circle, rewrite sine and cosine in terms of `z=e^{i\theta}`, and let residues do the rest.

---

## REQUIRED SECTIONS

### 1. Why Complex Methods Help
Explain why trigonometric definite integrals can be converted into contour integrals.

### 2. The Standard Substitution
Present clearly:
- `z=e^{i\theta}`
- `\cos\theta = \frac{1}{2}\left(z+\frac{1}{z}\right)`
- `\sin\theta = \frac{1}{2i}\left(z-\frac{1}{z}\right)`
- `d\theta = \frac{dz}{iz}`
Explain mapping of `0\le \theta \le 2\pi` to the unit circle.

### 3. General Strategy
Step-by-step conversion of `\int_0^{2\pi} R(\cos\theta,\sin\theta)\,d\theta` into a contour integral.

### 4. Identifying Poles Inside the Unit Circle
Explain the importance of selecting only poles with `|z|<1`.

### 5. Worked Examples
At least 8 examples including classic forms such as:
- `\int_0^{2\pi} \frac{d\theta}{a+b\cos\theta}` (with condition `a>|b|`)
- one sine-containing rational example
- one example with symmetry simplification
- one example where pole-selection inside unit circle is emphasized
Each example ends with learnbox.

### 6. Conversion Table (MANDATORY UPGRADE)
Table: trigonometric expression | complex substitution form.

### 7. Pole-Selection Diagram (MANDATORY UPGRADE)
Include a unit-circle diagram showing poles inside and outside the contour.

### 8. Excel Example (MANDATORY)
Numerically approximate a trigonometric integral and compare with the residue-theorem result.

### 9. Python Example (MANDATORY)
Numerically evaluate a definite integral and compare with the exact complex-analysis result.

### 10. Viva Questions (8)
### 11. Descriptive Questions (5)
### 12. Practice Problems (6)
### 13. MCQs (5)
### 14. Common Mistakes
Include wrong substitution formulas, forgetting `d\theta = dz/(iz)`, selecting poles outside the unit circle, and algebra errors when simplifying rational expression in `z`.

### 15. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Standard substitution formulas included
- [ ] Unit-circle mapping explained
- [ ] At least 8 worked examples
- [ ] Conversion table included
- [ ] Pole-selection diagram included
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
