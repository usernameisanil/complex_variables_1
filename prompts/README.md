# Prompts — Complex Variables Units I & II

This folder contains one detailed prompt file per topic. Each prompt is designed to be pasted into an AI model (Claude, GPT-4, etc.) to generate a complete LaTeX-formatted topic note.

## Folder Structure

```
prompts/
├── README.md                    ← This file
├── prompt_to_generate_response.txt  ← Master instructions for AI generation
├── unit_i/                      ← Unit I prompts (Topics 01–08)
└── unit_ii/                     ← Unit II prompts (Topics 09–19)
```

## How to Use

1. Open the relevant `topic_NN_*.md` file
2. Copy the full prompt
3. Paste into an AI assistant
4. Save the output `.tex` file in `responses/`
5. Compile with `pdflatex`

## Topic Index

### Unit I — Differentiation
| File | Topic |
|------|-------|
| `unit_i/topic_01_intro_functions_complex_variable.md` | Introduction to Functions of Complex Variable |
| `unit_i/topic_02_limit_continuity.md` | Concept of Limit & Continuity |
| `unit_i/topic_03_differentiation.md` | Differentiation |
| `unit_i/topic_04_cauchy_riemann_equations.md` | Cauchy-Riemann Equations |
| `unit_i/topic_05_analytic_functions.md` | Analytic Functions |
| `unit_i/topic_06_harmonic_functions.md` | Harmonic Functions |
| `unit_i/topic_07_harmonic_conjugate.md` | Finding Harmonic Conjugate |
| `unit_i/topic_08_milne_thomson_method.md` | Milne Thomson Method |

### Unit II — Integration
| File | Topic |
|------|-------|
| `unit_ii/topic_09_line_integral.md` | Line Integral |
| `unit_ii/topic_10_contour_integration.md` | Contour Integration |
| `unit_ii/topic_11_cauchy_integral_theorem.md` | Cauchy's Integral Theorem |
| `unit_ii/topic_12_cauchy_integral_formula.md` | Cauchy Integral Formula |
| `unit_ii/topic_13_taylor_series.md` | Taylor's Series |
| `unit_ii/topic_14_zeros_analytic_functions.md` | Zeros of Analytic Functions |
| `unit_ii/topic_15_singularities.md` | Singularities |
| `unit_ii/topic_16_laurent_series.md` | Laurent's Series |
| `unit_ii/topic_17_residues.md` | Residues |
| `unit_ii/topic_18_cauchy_residue_theorem.md` | Cauchy Residue Theorem |
| `unit_ii/topic_19_definite_integrals_sine_cosine.md` | Definite Integrals: Sine and Cosine |
