# Prompt — Topic 18: Cauchy Residue Theorem (Without Proof)

**Unit:** II — Complex Variable: Integration  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 18: **Cauchy Residue Theorem (Without Proof)**. Since the syllabus explicitly says without proof, focus on intuitive meaning, usage steps, and problem-solving efficiency.

Use the same LaTeX framework and style as previous prompts.

Set:
- `\lhead{Topic 18: Cauchy Residue Theorem}`
- `\rhead{Unit II — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: A contour integral around a closed curve may seem difficult at first glance. But the Residue Theorem turns the entire problem into a finite checklist: find the singularities inside the contour, compute their residues, add them up, and multiply by `2\pi i`.

---

## REQUIRED SECTIONS

### 1. Big Idea of the Theorem
Explain why local residue information determines a global contour integral.

### 2. Statement of the Residue Theorem
State the theorem clearly, without proof, with all assumptions.

### 3. Step-by-Step Procedure for Use
Provide an algorithm:
1. identify singularities
2. select those inside contour
3. compute residues
4. sum them
5. multiply by `2\pi i`

### 4. Orientation and Sign
Explain positive orientation and what changes with reverse orientation.

### 5. Connection with Earlier Topics
Relate to contour integration, singularities, Laurent series, and residues.

### 6. Worked Examples
At least 8 examples including:
- rational function over a circle
- example with more than one pole inside
- example with one pole outside contour
- orientation reversal example
Each example ends with learnbox.

### 7. Problem-Solving Flowchart (MANDATORY UPGRADE)
Include a flowchart or decision tree for applying the theorem.

### 8. Excel Example (MANDATORY)
Organize singularities, pole locations, inside/outside test, and residue values in a spreadsheet-style table.

### 9. Python Example (MANDATORY)
Use sympy to locate poles and compute residues for a sample integrand.

### 10. Viva Questions (8)
### 11. Descriptive Questions (5)
### 12. Practice Problems (6)
### 13. MCQs (5)
### 14. Common Mistakes
Include summing residues outside contour, forgetting `2\pi i`, sign errors from orientation, and misclassifying poles.

### 15. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Theorem statement included
- [ ] No proof section included
- [ ] Step-by-step procedure included
- [ ] At least 8 worked examples
- [ ] Flowchart included
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
