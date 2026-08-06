# Complex Variables — Units I & II

**Course:** Complex Variables and Special Functions  
**University:** JNTUA College of Engineering (Autonomous), Ananthapuramu  
**Department:** Engineering Mathematics | B.Tech (R23)  

---

## About This Repository

This repository contains structured learning materials for **Units I and II** of the Complex Variables course — covering Complex Differentiation (Analytic Functions, Cauchy-Riemann Equations, Harmonic Functions) and Complex Integration (Line Integrals, Cauchy's Theorem, Laurent Series, Residues).

It mirrors the structure of [statistical_methods_1](https://github.com/usernameisanil/statistical_methods_1), with beginner-friendly, LaTeX-based topic notes.

---

## Repository Structure

```
complex_variables_1/
├── README.md                    ← This file
├── topics.txt                   ← All unit-wise topics in order
├── topics/                      ← Topic overview markdown files (unit-wise)
│   ├── unit_i_topics.md
│   └── unit_ii_topics.md
├── prompts/                     ← One detailed prompt per topic
│   ├── README.md
│   ├── prompt_to_generate_response.txt
│   ├── unit_i/
│   │   ├── topic_01_intro_functions_complex_variable.md
│   │   ├── topic_02_limit_continuity.md
│   │   ├── topic_03_differentiation.md
│   │   ├── topic_04_cauchy_riemann_equations.md
│   │   ├── topic_05_analytic_functions.md
│   │   ├── topic_06_harmonic_functions.md
│   │   ├── topic_07_harmonic_conjugate.md
│   │   └── topic_08_milne_thomson_method.md
│   └── unit_ii/
│       ├── topic_09_line_integral.md
│       ├── topic_10_contour_integration.md
│       ├── topic_11_cauchy_integral_theorem.md
│       ├── topic_12_cauchy_integral_formula.md
│       ├── topic_13_taylor_series.md
│       ├── topic_14_zeros_analytic_functions.md
│       ├── topic_15_singularities.md
│       ├── topic_16_laurent_series.md
│       ├── topic_17_residues.md
│       ├── topic_18_cauchy_residue_theorem.md
│       └── topic_19_definite_integrals_sine_cosine.md
└── responses/                   ← Placeholder .tex + .pdf for each topic
    ├── topic_01.tex
    └── ...
```

---

## Units Covered

### Unit I — Complex Variable: Differentiation
| # | Topic |
|---|-------|
| 01 | Introduction to Functions of Complex Variable |
| 02 | Concept of Limit & Continuity |
| 03 | Differentiation |
| 04 | Cauchy-Riemann Equations |
| 05 | Analytic Functions |
| 06 | Harmonic Functions |
| 07 | Finding Harmonic Conjugate |
| 08 | Construction of Analytic Function by Milne Thomson Method |

### Unit II — Complex Variable: Integration
| # | Topic |
|---|-------|
| 09 | Line Integral |
| 10 | Contour Integration |
| 11 | Cauchy's Integral Theorem (Simple Case) |
| 12 | Cauchy Integral Formula |
| 13 | Power Series Expansions: Taylor's Series |
| 14 | Zeros of Analytic Functions |
| 15 | Singularities |
| 16 | Laurent's Series |
| 17 | Residues |
| 18 | Cauchy Residue Theorem (Without Proof) |
| 19 | Evaluation of Definite Integral Involving Sine and Cosine |

---

## How to Use

1. Navigate to `prompts/unit_i/` or `prompts/unit_ii/` and open any topic file
2. Copy the prompt block inside the triple-backtick block
3. Paste into an AI model (e.g., Claude, GPT-4) to generate the LaTeX response
4. Save the output as the corresponding `.tex` file in `responses/`
5. Compile with `pdflatex` to get the final PDF

---

## Textbooks Referenced

1. B.S. Grewal — *Higher Engineering Mathematics*, Khanna Publishers, 44th Edition
2. Erwin Kreyszig — *Advanced Engineering Mathematics*, 10th Edition, Wiley
3. R.K. Jain & S.R.K. Iyengar — *Advanced Engineering Mathematics*, Narosa Publishing
4. Churchill & Brown — *Complex Variables and Applications*, McGraw-Hill

---

## Online Resources

- https://nptel.ac.in/courses/111106084
- https://nptel.ac.in/courses/111107056
- https://ocw.mit.edu/courses/18-04-complex-variables-with-applications-spring-2018/
