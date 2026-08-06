# Prompt — Topic 10: Contour Integration

**Unit:** II — Complex Variable: Integration  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 10: **Contour Integration**. Build naturally from line integrals and help students understand contours, orientation, and closed paths.

Use the same LaTeX structure and pedagogical style as earlier prompts.

Set:
- `\lhead{Topic 10: Contour Integration}`
- `\rhead{Unit II — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: If a line integral follows any curve, then a contour integral is the next big step: the curve may close into a loop. Once the path closes, extraordinary theorems begin to appear — and they become the foundation of complex integration.

---

## REQUIRED SECTIONS

### 1. From Line Integral to Contour Integral
Explain the idea of integrating along closed and piecewise smooth curves.

### 2. Definition of Contour and Contour Integral
Define contour, simple contour, closed contour, simple closed contour, positively oriented contour.

### 3. Standard Contours
Discuss circles, semicircles, rectangles, triangles, and piecewise contours commonly used in problems.
Include a diagram showing several standard contour types.

### 4. Orientation and Its Effect
Explain clockwise vs counterclockwise orientation and sign change under reversal.

### 5. Evaluating Contour Integrals by Parametrization
Show at least 3 model parametrizations:
- unit circle
- upper semicircle
- straight-line segment

### 6. Connection with Path Dependence
Explain when contour integrals may depend on the path and how this motivates later theorems.

### 7. Worked Examples
At least 6 examples including:
- `\oint_C z\,dz` over a circle
- `\oint_C 1/z\,dz` over unit circle
- piecewise contour example
- orientation reversal example
Every example ends with learnbox.

### 8. Contour Catalogue Table (MANDATORY UPGRADE)
Provide a compact table: contour type | parametrization | interval for parameter | orientation.

### 9. Excel Example (MANDATORY)
Numerically sample points on a circle or rectangle and approximate contour integrals.

### 10. Python Example (MANDATORY)
Plot a contour and numerically integrate a function around it.

### 11. Viva Questions (8)
### 12. Descriptive Questions (5)
### 13. Practice Problems (6)
### 14. MCQs (5)
### 15. Common Mistakes
Include wrong orientation, incorrect circle parametrization, forgetting piecewise splitting, and mixing contour with region.

### 16. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Contour definitions included
- [ ] Standard contour diagram included
- [ ] At least 6 worked examples
- [ ] Contour catalogue table included
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
