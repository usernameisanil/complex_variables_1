# Prompt — Topic 11: Cauchy's Integral Theorem (Simple Case)

**Unit:** II — Complex Variable: Integration  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 11: **Cauchy's Integral Theorem (Simple Case)**. Students should understand the statement, intuition, simple proof idea, and its consequences.

Use the same LaTeX framework and conversational teaching style as the previous prompts.

Set:
- `\lhead{Topic 11: Cauchy Integral Theorem}`
- `\rhead{Unit II — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: Imagine walking around a closed loop while measuring a complex-valued quantity along the way. In ordinary calculus, there is no reason for the total to vanish. But in complex analysis, if the function is analytic and the region is nice enough, the entire closed integral collapses to zero. That is one of the most beautiful surprises in mathematics.

---

## REQUIRED SECTIONS

### 1. Why This Theorem Matters
Explain its role as the foundation of contour integration and later results.

### 2. Statement of the Theorem
State the simple-case theorem clearly for analytic functions in a simply connected region.

### 3. Meaning of Simply Connected Region
Explain with examples and diagrams: disk, annulus, punctured plane.

### 4. Proof Idea (Simple Case)
Give a student-friendly proof outline using `f(z)=u+iv`, decomposition into real integrals, Green's theorem, and C-R equations. Keep it accessible.

### 5. Consequences
Include:
- closed integral is zero
- path independence in simply connected domains
- existence of antiderivative

### 6. When the Theorem Fails
Discuss singularity inside the contour, non-simply-connected setting, and why `1/z` is the classic caution example.

### 7. Worked Examples
At least 7 examples, including:
- analytic polynomial over closed contour
- `1/z` over unit circle as failure case
- comparison of two paths between same endpoints in analytic region
- piecewise contour example
Each example ends with learnbox.

### 8. Region-Type Comparison (MANDATORY UPGRADE)
Table: region/function condition | theorem applies? | reason.

### 9. Excel Example (MANDATORY)
Numerical approximation around a closed curve for an analytic polynomial and comparison with a non-analytic / singular case.

### 10. Python Example (MANDATORY)
Approximate contour integrals for two cases, one giving near zero and one not.

### 11. Viva Questions (8)
### 12. Descriptive Questions (5)
### 13. Practice Problems (6)
### 14. MCQs (5)
### 15. Common Mistakes
Include assuming theorem works for every closed contour, ignoring singularities inside contour, confusion about simply connected domains.

### 16. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Theorem statement included
- [ ] Simply connected region explained with diagrams
- [ ] Proof idea included
- [ ] Failure case `1/z` included
- [ ] At least 7 worked examples
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
