# Prompt — Topic 08: Construction of Analytic Function by Milne Thomson Method

**Unit:** I — Complex Variable: Differentiation  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

Write a **complete, compilable LaTeX lecture note** for Topic 08: **Construction of Analytic Function by Milne Thomson Method**. This should feel like the natural climax of Unit I: students have learned analytic functions, C-R equations, harmonic functions, and harmonic conjugates, and now they learn a direct construction technique.

Use the same LaTeX framework and style as earlier prompts.

Set fancyhdr:
- `\lhead{Topic 08: Milne Thomson Method}`
- `\rhead{Unit I — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK
Inside curiositybox: Up to now, finding an analytic function often meant first hunting down the harmonic conjugate. Milne Thomson's method offers a shortcut: instead of reconstructing the missing part step by step, it builds the analytic function directly.

---

## REQUIRED SECTIONS

### 1. Why This Method Is Useful
Explain how it improves on the harmonic-conjugate approach in some problems.

### 2. Background Needed
Briefly recap `f(z)=u+iv`, C-R equations, and harmonic conjugates.

### 3. Milne Thomson Method When `u(x,y)` Is Given
Derive/show formula in a student-friendly manner.
Explain substitution `x=z, y=0` carefully.

### 4. Milne Thomson Method When `v(x,y)` Is Given
Give the parallel procedure.

### 5. Step-by-Step Algorithm
Present a structured algorithm students can memorize and apply.

### 6. Worked Examples
At least 8 examples including:
- given `u=x^2-y^2`
- given `u=e^x\cos y`
- given `v=2xy`
- rational-form example
- example compared with harmonic-conjugate method to confirm same answer
Every example ends with learnbox.

### 7. Comparison with Harmonic Conjugate Method (MANDATORY UPGRADE)
Provide a short comparison table: Method | Advantages | Limitations | Best use case.

### 8. Flowchart / Algorithm Summary (MANDATORY UPGRADE)
Include a clear flowchart or numbered decision process.

### 9. Excel Example (MANDATORY)
Show how a spreadsheet can organize derivative calculations and substitutions.

### 10. Python Example (MANDATORY)
Use sympy to automate partial derivatives and the substitution step for one example.

### 11. Viva Questions (8)
### 12. Descriptive Questions (5)
### 13. Practice Problems (6)
### 14. MCQs (5)
### 15. Common Mistakes
Include wrong substitution of `x=z, y=0`, sign mistakes, forgetting integration constant, and applying method without first ensuring consistency.

### 16. Quick Recap

---

## MANDATORY QUALITY CHECKLIST
- [ ] Both u-given and v-given methods included
- [ ] Step-by-step algorithm included
- [ ] At least 8 worked examples
- [ ] Comparison with harmonic conjugate method included
- [ ] Flowchart or algorithm summary included
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
