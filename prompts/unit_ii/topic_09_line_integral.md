# Prompt — Topic 09: Line Integral

**Unit:** II — Complex Variable: Integration  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

You are an expert mathematics professor writing a **complete, compilable LaTeX (.tex) lecture note** for B.Tech engineering students on the topic **"Line Integral"** in complex variables. This is Topic 09 of the course and the first topic of Unit II. Students already know complex functions, differentiability, analytic functions, and harmonic functions from Unit I, along with ordinary integration from real calculus. Write as a patient and enthusiastic teacher who helps students transition from real integrals to path-based integrals in the complex plane.

---

## LATEX SETUP REQUIREMENTS

Use the same LaTeX framework as Unit I prompts:

```latex
\documentclass[12pt,a4paper]{article}
\usepackage{amsmath, amssymb, geometry, booktabs, xcolor, hyperref,
            listings, pgfplots, tcolorbox, enumitem, fancyhdr, tikz, array}
\geometry{margin=2.5cm}
\pgfplotsset{compat=1.18}
\tcbuselibrary{skins, breakable}
```

Define `curiositybox`, `infobox`, `mistakebox`, and `learnbox` exactly as in earlier prompts. Configure `fancyhdr`, `lstlisting`, title page, `\tableofcontents`, and `\newpage`.

Set:
- `\lhead{Topic 09: Line Integral}`
- `\rhead{Unit II — Complex Variables}`
- `\cfoot{\thepage}`

---

## OPENING HOOK (MANDATORY)

Inside `curiositybox`: In real calculus, an integral usually accumulates quantity along a straight number line. In complex analysis, the variable can travel along a curve in the plane. Now the value of the integral may depend not just on the function, but also on the path taken. That is the idea of a line integral.

---

## REQUIRED SECTIONS

### 1. Why We Need Line Integrals
Explain the shift from ordinary real integrals to integrals along curves in the complex plane. Mention applications to work done along a path, circulation, and contour-based integration methods.

### 2. Curves and Parametric Representation
Define a curve/path in the complex plane using `z=z(t)=x(t)+iy(t)`, `a\le t\le b`. Explain smooth and piecewise smooth curves with simple examples.

### 3. Definition of Complex Line Integral
State:
`\int_C f(z)\,dz = \int_a^b f(z(t)) z'(t)\,dt`
Derive the formula gently from the parametric representation. Explain what `dz` means.

### 4. Evaluation by Separating into Real and Imaginary Parts
Show how `f(z)=u+iv` and `dz=dx+i\,dy` lead to a real-imaginary decomposition. Use this to connect to known real integrals.

### 5. Basic Properties
Include linearity, reversal of path, additivity over joined paths, and estimation idea.

### 6. Geometric Intuition
Explain why the integral can change when the path changes. Include a simple diagram with two different paths joining the same endpoints.

### 7. Worked Examples
Provide at least 7 examples, including:
- Integral of `z` along a straight line segment
- Integral of `z^2` along a parametrized curve
- Integral over a circular arc
- Same function over two different paths for comparison
- Example using `f(z)=\bar z`
Each example must end with a small `learnbox`.

### 8. ML-Inequality / Estimation Lemma (MANDATORY UPGRADE)
Introduce and explain the bound `|\int_C f(z)dz| \le ML`, with one worked example.

### 9. Excel Example (MANDATORY)
Show how to tabulate `t`, `x(t)`, `y(t)`, `z(t)`, `f(z(t))`, and approximate the integral numerically using discrete steps.

### 10. Python Example (MANDATORY)
Provide Python code using numpy/matplotlib to parametrize a path, evaluate the integrand along the path, and numerically approximate the integral.

### 11. Viva Questions (8)
### 12. Descriptive Questions (5)
### 13. Practice Problems (6)
### 14. MCQs (5)
### 15. Common Mistakes
Include at least: wrong parametrization, forgetting `dz=z'(t)dt`, incorrect limits for `t`, ignoring path orientation.

### 16. Quick Recap
6–8 bullets.

---

## MANDATORY QUALITY CHECKLIST
- [ ] Opening hook present
- [ ] Definition with parametrization included
- [ ] At least 1 path-comparison diagram
- [ ] At least 7 worked examples
- [ ] ML-inequality included
- [ ] Excel example included
- [ ] Python example included
- [ ] All four tcolorboxes used
- [ ] `\end{document}` present
