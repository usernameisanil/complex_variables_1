# Prompt — Topic 01: Introduction to Functions of Complex Variable

**Unit:** I — Complex Variable: Differentiation  
**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous)  
**Target Audience:** B.Tech engineering students  

---

## Prompt

You are an expert mathematics professor writing a **complete, compilable LaTeX (.tex) lecture note** for B.Tech engineering students on the topic **"Introduction to Functions of Complex Variable"**. This is Topic 01 of Unit I. Students know basic algebra, coordinate geometry, and elementary complex numbers, but are new to complex analysis. Write as an enthusiastic, patient teacher who makes the subject feel visual, intuitive, and connected to familiar real-variable ideas.

---

## LATEX SETUP REQUIREMENTS

Use this exact preamble (add any extra packages needed by the content):

```latex
\documentclass[12pt,a4paper]{article}
\usepackage{amsmath, amssymb, geometry, booktabs, xcolor, hyperref,
            listings, pgfplots, tcolorbox, enumitem, fancyhdr, tikz, array}
\geometry{margin=2.5cm}
\pgfplotsset{compat=1.18}
\tcbuselibrary{skins, breakable}
```

Define these four tcolorbox environments in the preamble:
- `\newtcolorbox{curiositybox}` — colback=yellow!10, colframe=orange!80
- `\newtcolorbox{infobox}` — colback=blue!5, colframe=blue!60
- `\newtcolorbox{mistakebox}` — colback=red!5, colframe=red!60
- `\newtcolorbox{learnbox}` — colback=green!5, colframe=green!60

Set up fancyhdr with:
- `\lhead{Topic 01: Functions of Complex Variable}`
- `\rhead{Unit I — Complex Variables}`
- `\cfoot{\thepage}`

Configure lstlisting for Python with standard readable settings.

Title page: `\title{Topic 01: Introduction to Functions of Complex Variable \\ \large Unit I — Complex Variable: Differentiation}`, `\maketitle`, then `\tableofcontents`, then `\newpage`.

---

## AUDIENCE AND TONE

- Students are capable but may be uneasy when mathematics becomes abstract.
- Explain like a friendly teacher who constantly connects new ideas to already-known concepts.
- Use energetic phrases like: "Here is the key idea", "Let us visualize this", "This looks new, but notice the pattern".
- Keep explanations clear, layered, and example-driven.

---

## OPENING HOOK (MANDATORY)

Place inside `\begin{curiositybox}[Hook]`: In real-variable calculus, we input one real number and get one real output. But what if both the input and output have two parts — real and imaginary? Suddenly, a function does not just draw a curve; it can transform an entire plane. That is the world of complex variables.

---

## REQUIRED SECTIONS

### 1. Why This Topic Matters
Explain why complex variables are important in engineering mathematics, signal processing, fluid flow, electromagnetics, and conformal mapping. Include a two-column table: "If we stop at real functions" vs "What complex functions allow us to do". End with a learnbox.

### 2. Recap of Complex Numbers
Cover:
- Definition of complex number `z = x + iy`
- Real part, imaginary part
- Equality of complex numbers
- Addition, subtraction, multiplication
- Complex conjugate
- Modulus and amplitude
- Polar form `z = r(\cos \theta + i \sin \theta)`
Include worked examples.

### 3. Argand Plane
Explain plotting complex numbers on the plane, geometric meaning of modulus and argument, and relation between Cartesian and polar forms.
- Include one **TikZ or pgfplots diagram** showing several points in the Argand plane.
- Include one infobox of core formulas.

### 4. Functions of a Complex Variable
Define `w = f(z)` where `z = x + iy` and `w = u(x,y) + iv(x,y)`.
Explain that one complex function is equivalent to two real-valued functions.
Include several examples:
- `f(z) = z^2`
- `f(z) = z + 1/z`
- `f(z) = e^z` (introductory level only)
For each, derive real and imaginary parts.

### 5. Standard Transformations / Mapping Idea
Introduce the idea that a complex function maps points from the z-plane to the w-plane.
Use examples:
- Translation by `w = z + c`
- Scaling and rotation by `w = az`
- Squaring map `w = z^2`
Explain geometrically what happens to lines/circles in simple terms.

### 6. Algebra of Complex Functions
Explain sum, difference, product, quotient, composition of complex functions.
Give at least 3 worked examples.

### 7. Worked Examples
Provide at least 5 substantial examples, including:
- Writing a function in `u + iv` form
- Finding modulus and argument of a function value
- Converting between Cartesian and polar forms
- Identifying domain restrictions for `1/z` and `1/(z-1)`
- Mapping of a simple line or circle under a basic transformation
Every example must end with a small learnbox.

### 8. Excel Example (MANDATORY)
Show how a spreadsheet can store columns for `x`, `y`, `u(x,y)`, `v(x,y)`, modulus, and argument for a function like `f(z)=z^2`. Include sample formulas.

### 9. Python Example (MANDATORY)
Provide a Python script that:
- Generates several complex numbers
- Computes `f(z)=z^2`
- Prints real and imaginary parts
- Plots input and output points on separate axes using matplotlib
Include expected output as comments.

### 10. Viva Questions (8)
Short oral questions on modulus, argument, conjugate, Argand plane, polar form, and `u+iv` representation.

### 11. Descriptive Questions (5)
Exam-style theory questions covering complex number basics, Argand plane, function representation, and mappings.

### 12. Practice Problems (6)
Numerical and conceptual problems with short answer hints.

### 13. MCQs (5)
4 options each, bold the correct answer, one-line explanation.

### 14. Common Mistakes
Use a mistakebox table with at least 4 rows, including:
- Confusing imaginary part with coefficient of `i`
- Wrong modulus formula
- Treating argument as unique without mentioning principal value / multiple values
- Algebra mistakes in expanding `(x+iy)^2`

### 15. Quick Recap
6–8 bullets with formulas and takeaways.

---

## MANDATORY QUALITY CHECKLIST

- [ ] Opening hook present
- [ ] At least 1 Argand plane diagram
- [ ] At least 1 booktabs table with 4+ rows
- [ ] At least 1 Excel example
- [ ] At least 1 Python example
- [ ] At least 5 worked examples
- [ ] All four tcolorbox environments used
- [ ] `\end{document}` present
- [ ] No undefined LaTeX macros
