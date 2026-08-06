# Complex Variables Lecture Note Generation -- Execution Meta-Prompt (Self-Driving)

**Repo:** `usernameisanil/complex_variables_1`
**Branch:** `main`
**Prompts directory:** `prompts/unit_i/` and `prompts/unit_ii/`
**Responses directory:** `responses/unit_i/` and `responses/unit_ii/`

---

## PURPOSE

This is the **one and only prompt** you need to run for every topic.
You do NOT copy-paste any topic file. The LLM reads it from GitHub directly.

### How to trigger a run

Start a new session with an LLM that has GitHub MCP access, then send:

```
Read EXECUTION_META_PROMPT.md from the repo usernameisanil/complex_variables_1,
follow it exactly, and process this topic file:
prompts/unit_i/topic_01_intro_functions_complex_variable.md
```

Change the last filename for each of the 19 topics. That is all.

---

## ALL 19 TOPIC FILES (for reference)

### Unit I -- Functions of a Complex Variable and Analytic Functions
1. `prompts/unit_i/topic_01_intro_functions_complex_variable.md`
2. `prompts/unit_i/topic_02_limit_continuity.md`
3. `prompts/unit_i/topic_03_differentiation.md`
4. `prompts/unit_i/topic_04_cauchy_riemann_equations.md`
5. `prompts/unit_i/topic_05_analytic_functions.md`
6. `prompts/unit_i/topic_06_harmonic_functions.md`
7. `prompts/unit_i/topic_07_harmonic_conjugate.md`
8. `prompts/unit_i/topic_08_milne_thomson_method.md`

### Unit II -- Complex Integration and Series
9.  `prompts/unit_ii/topic_09_line_integral.md`
10. `prompts/unit_ii/topic_10_contour_integration.md`
11. `prompts/unit_ii/topic_11_cauchy_integral_theorem.md`
12. `prompts/unit_ii/topic_12_cauchy_integral_formula.md`
13. `prompts/unit_ii/topic_13_taylor_series.md`
14. `prompts/unit_ii/topic_14_zeros_analytic_functions.md`
15. `prompts/unit_ii/topic_15_singularities.md`
16. `prompts/unit_ii/topic_16_laurent_series.md`
17. `prompts/unit_ii/topic_17_residues.md`
18. `prompts/unit_ii/topic_18_cauchy_residue_theorem.md`
19. `prompts/unit_ii/topic_19_evaluation_definite_integrals.md`

---

# INSTRUCTIONS FOR THE LLM

You are reading this file because the user asked you to process a specific topic.
Follow every step below in strict sequence. Do not skip any step.

---

## STEP 0: AUTHENTICATE AND READ THE TOPIC FILE

Using your GitHub MCP tool:

1. Call `get_file_contents` with:
   - `owner`: `usernameisanil`
   - `repo`: `complex_variables_1`
   - `path`: *(the topic file path the user specified)*
2. Read the returned content **completely and carefully** before writing a single line of LaTeX.
3. Extract and note these values from the prompt file:

| What to extract | Where to find it |
|----------------|------------------|
| Topic name | First heading or `**Unit:**` line |
| Unit number | `**Unit:**` line |
| Unit title | `**Unit:**` line |
| N = number of atomic sub-topics | Count rows in the Section 0 table |
| Exact `\lhead{}` value | Section 1 preamble block |
| Exact `\rhead{}` value | Section 1 preamble block |
| Exact `\title{}` value | Section 1 preamble block |
| Output filename | Same as prompt filename, replace `.md` with `.tex` |

Output filename mapping examples:
- Input: `prompts/unit_i/topic_04_cauchy_riemann_equations.md`
- Output: `responses/unit_i/topic_04_cauchy_riemann_equations.tex`

- Input: `prompts/unit_ii/topic_16_laurent_series.md`
- Output: `responses/unit_ii/topic_16_laurent_series.tex`

**Do not proceed to Step 1 until you have read and understood the entire topic file.**

---

## STEP 1: GENERATE THE COMPLETE LaTeX FILE

Generate the **complete, fully written, self-contained LaTeX source file**
following every instruction in the topic file with zero omissions.

### 1a. Structure Rules (Non-Negotiable)

1. **Start with the exact preamble** from Section 1 of the topic file -- copy verbatim.
   For Topics 02--19 that reference Topic 01's preamble, use the following canonical preamble:

```latex
\documentclass[12pt,a4paper]{article}
\usepackage{amsmath,amssymb,amsthm}
\usepackage{geometry}
\geometry{margin=1in}
\usepackage{booktabs}
\usepackage{array}
\usepackage{enumitem}
\usepackage{fancyhdr}
\usepackage{tcolorbox}
\tcbuselibrary{skins,breakable}
\usepackage{pgfplots}
\pgfplotsset{compat=1.18}
\usepackage{tikz}
\usetikzlibrary{arrows.meta,positioning,shapes.geometric,calc}
\usepackage{xcolor}
\usepackage{hyperref}
\hypersetup{colorlinks=true, linkcolor=blue, urlcolor=blue}

\newtcolorbox{infobox}[1]{colback=blue!5!white, colframe=blue!60!black, fonttitle=\bfseries, title=#1, breakable}
\newtcolorbox{curiositybox}[1]{colback=orange!10!white, colframe=orange!80!black, fonttitle=\bfseries, title=#1, breakable}
\newtcolorbox{learnbox}[1]{colback=green!5!white, colframe=green!50!black, fonttitle=\bfseries, title=#1, breakable}
\newtcolorbox{mistakebox}[1]{colback=red!5!white, colframe=red!60!black, fonttitle=\bfseries, title=#1, breakable}

\pagestyle{fancy}
\fancyhf{}
\lhead{<TOPIC-SPECIFIC VALUE FROM PROMPT FILE>}
\rhead{<TOPIC-SPECIFIC VALUE FROM PROMPT FILE>}
\cfoot{\thepage}
```

   Always substitute the exact `\lhead{}` and `\rhead{}` values from the topic file.

2. After `\begin{document}`, write `\maketitle` then `\tableofcontents` then `\newpage`.
3. **Generate ALL 10 sections** in this exact order:
   - Section 1: Real-World Engineering Hook (curiositybox)
   - Section 2: Why This Topic Exists (booktabs table + learnbox)
   - Section 3: Intuition + Definitions -- **exactly N subsections**, one per atomic sub-topic
   - Section 4: Visual Artifacts (TikZ / pgfplots diagrams)
   - Section 5: Step-by-Step Algorithmic Workflow
   - Section 6: Fully Worked Numerical Examples
   - Section 7: Tabular Reference / Comparison
   - Section 8: Common Mistakes (mistakebox tabular)
   - Section 9: Assessment Suite (Viva + Descriptive + Practice Problems + MCQ)
   - Section 10: Quick Recap and Formula Sheet (learnbox)
4. **Section 3 must contain exactly N `\subsection{}` entries** -- one per row in the Section 0 table.
   Never merge two sub-topics. Never add extra sub-topics not in the table.
5. Each subsection must follow this internal order:
   - 2--3 lines of conversational intuition (plain text)
   - `infobox` with all formal definitions, theorems, formulas, properties
   - At least one dedicated worked example with full step-by-step arithmetic

### 1b. Content Rules (Non-Negotiable)

6. Every **infobox** must contain the exact definitions and formulas listed in the
   Section 0 table for that sub-topic. No generic placeholders.
7. Every **worked example** must use distinct numerical values not reused across examples.
   Show every arithmetic step. Never write:
   - "it can be shown"
   - "the reader can verify"
   - "similarly"
   - "(details omitted)"
   - "continuing in the same way"
8. **Section 2 table**: one row per atomic sub-topic, genuine engineering consequence per row.
9. **Section 7 table**: revision-useful, topic-specific -- not a copy of Section 3.
10. **Section 8 mistakebox tabular**: minimum one row per atomic sub-topic (>= N rows).
11. **Section 9 assessment** must meet ALL minimums from the topic file enforcement rules.
    Typical minimums: viva >= 8, descriptive >= 5, practice problems >= 6, MCQ >= 5.
    MCQs: 4 options each, bold correct answer with `\textbf{}`, one-line explanation.
12. **Section 10 learnbox**: exactly the bullet count specified in the topic file (usually 6--10).
    Each bullet must be topic-specific -- not generic math advice.
13. **Engineering hook (Section 1)**: must describe a specific realistic application scenario
    by name (e.g., "signal processing using the residue theorem", "conformal mapping in
    airfoil design", "AC circuit analysis using complex impedance").
    Never write "mathematics is important for engineers."
14. **Complex variables specific**: all complex numbers use $z = x + iy$ notation.
    Use $\operatorname{Re}(z)$ and $\operatorname{Im}(z)$ for real and imaginary parts.
    Use $\overline{z}$ for complex conjugate. Use $|z|$ for modulus.
    Use $\arg(z)$ for argument. Polar form: $z = re^{i\theta} = r(\cos\theta + i\sin\theta)$.

### 1c. LaTeX Correctness Rules (Non-Negotiable)

15. **Complex integrals**: use `\oint` for contour integrals, `\int` for line integrals.
    Contour integration: `\oint_{C} f(z)\,dz`
16. **pmatrix for all matrices:**
    `\begin{pmatrix} a & b \\\\ c & d \end{pmatrix}`
17. **tcolorbox syntax:** `\newtcolorbox{name}[1]{..., title=#1, breakable}`
    NOT `[1][]` -- the title argument is positional, not keyword.
18. **Every box opened must be closed:**
    `\begin{infobox}{Title}` ... `\end{infobox}`
    `\begin{curiositybox}{Title}` ... `\end{curiositybox}`
    `\begin{learnbox}{Title}` ... `\end{learnbox}`
    `\begin{mistakebox}{Title}` ... `\end{mistakebox}`
19. **No bare special characters in text mode:**
    - Use `\%` not `%`
    - Use `\$` not `$` in text
    - Use `\&` not `&` outside tabular
    - Use `\_` not `_` outside math
20. **No Unicode in LaTeX source:**
    - `---` not `--` not the Unicode em-dash character
    - `\geq` not `>=` or Unicode
    - `\leq`, `\to`, `\ldots`, `\cdot` not their Unicode equivalents
    - `\times` not the Unicode times character
    - `\pi` not the Unicode pi character
    - `\infty` not the Unicode infinity character
21. **TikZ and pgfplots visuals:**
    - Fully self-contained (no `\input{}`, no `\includegraphics{}`)
    - Every `\begin{tikzpicture}` closed with `\end{tikzpicture}`
    - Every `\begin{axis}` closed with `\end{axis}` inside tikzpicture
    - 3D surf plots: use `samples=40` maximum
    - Every axis: `xlabel`, `ylabel` at minimum
    - For Argand diagrams: use `\draw[->]` axes, `\filldraw` for points, label clearly
22. **Document boundaries:**
    - First line of file: `\documentclass[12pt,a4paper]{article}`
    - Last line of file: `\end{document}`
    - Nothing before `\documentclass`, nothing after `\end{document}`
23. **Never truncate:**
    Do not end any section with:
    - "(add more questions as needed)"
    - "(remaining sub-topics follow the same pattern)"
    - "..."
    - "etc."
    Every question, every row, every bullet must be fully written out.

---

## STEP 2: PRE-PUSH SELF-CHECK

Before pushing, verify every item in this checklist.
If any item fails, fix it before proceeding.

```
PRE-PUSH CHECKLIST
------------------
[ ] Preamble copied verbatim from topic file (lhead, rhead, title, packages)
[ ] \newtcolorbox uses [1] not [1][] -- verified
[ ] \begin{document} present immediately after preamble
[ ] \maketitle and \tableofcontents present after \begin{document}
[ ] Section 3 contains exactly N \subsection{} entries (N = from Step 0)
[ ] Every \begin{infobox}, \begin{learnbox}, \begin{curiositybox}, \begin{mistakebox} is closed
[ ] Every \begin{tikzpicture} is closed with \end{tikzpicture}
[ ] Every \begin{axis} is closed with \end{axis}
[ ] No bare _ or ^ outside math mode
[ ] No bare & outside tabular/align
[ ] No bare % in text (use \% or write percent)
[ ] No Unicode characters in LaTeX source
[ ] All N sub-topics have: infobox + worked example + assessment item
[ ] Section 8 mistakebox has >= N rows
[ ] Section 9 meets all count minimums from topic file
[ ] Section 10 learnbox has the exact bullet count specified
[ ] No section ends with placeholder text or ellipsis
[ ] Complex integrals use \oint for contour integrals
[ ] Complex notation uses z = x + iy, \operatorname{Re}, \operatorname{Im}, \overline{z}
[ ] \end{document} is the very last line
```

---

## STEP 3: PUSH TO GITHUB

Using your GitHub MCP tool, call `create_or_update_file` with:

| Parameter | Value |
|-----------|-------|
| `owner` | `usernameisanil` |
| `repo` | `complex_variables_1` |
| `branch` | `main` |
| `path` | `responses/unit_i/<output_filename>.tex` or `responses/unit_ii/<output_filename>.tex` |
| `message` | `response: <output_filename>.tex -- LaTeX lecture note for <Topic Name>, Unit <N>` |
| `content` | The complete .tex file as a string |

Path routing rule:
- Topics 01--08 go to: `responses/unit_i/<filename>.tex`
- Topics 09--19 go to: `responses/unit_ii/<filename>.tex`

If the file already exists in the repo (a previous attempt),
you MUST fetch its current SHA first using `get_file_contents`
and pass it as the `sha` parameter. Omitting SHA on an existing file will cause a 422 error.

**Do NOT push if any checklist item above is unchecked.**
Fix the issue, recheck, then push.

---

## STEP 4: REPORT COMPLETION

After a successful push, output this exact report:

```
===========================================
COMPLEX VARIABLES -- GENERATION COMPLETE
===========================================
File pushed : responses/<unit>/<output_filename>.tex
Commit SHA  : <sha from push response>
Commit URL  : <html_url from push response>
Topic       : <Topic Name>
Unit        : Unit <N> -- <Unit Title>
-------------------------------------------
Sub-topics covered (<N> total):
  1. <sub-topic 1 name>
  2. <sub-topic 2 name>
  ... (all N)
-------------------------------------------
Sections generated:
  1  Real-World Hook        [curiositybox]
  2  Why This Topic         [booktabs table + learnbox]
  3  Definitions            [N subsections x infobox]
  4  Visuals                [TikZ/pgfplots count: X]
  5  Algorithmic Workflow   [boxed steps]
  6  Worked Examples        [count: X]
  7  Reference Table        [booktabs]
  8  Common Mistakes        [mistakebox, X rows]
  9  Assessment             [viva: X | descriptive: X | practice: X | MCQ: X]
  10 Formula Sheet          [learnbox, X bullets]
-------------------------------------------
All checklist items: PASSED
===========================================
```

---

## KNOWN FAILURE MODES -- PREVENT THESE

| # | Failure | Prevention |
|---|---------|------------|
| 1 | `\newtcolorbox{infobox}[1][]` | Use `[1]` only -- not `[1][]` |
| 2 | Unclosed tcolorbox | Write `\end{infobox}` immediately after planning each box |
| 3 | Unicode em-dash in .tex | Type `---` not the Unicode character |
| 4 | 3D plot compilation timeout | `samples=40` maximum for surf plots |
| 5 | Wrong subsection count | Re-count rows in Section 0 table before writing Section 3 |
| 6 | Truncated assessment | Every question written in full -- no ellipsis, no "add more" |
| 7 | Missing `\maketitle` | Always: `\begin{document}` then `\maketitle` then `\tableofcontents` |
| 8 | SHA missing on update | Always fetch existing file SHA before pushing an update |
| 9 | Bare `%` in text | Write `\%` or spell out "percent" |
| 10 | Mixed notation | Use `\oint` for contour integrals throughout; never `\int` for closed curves |
| 11 | Wrong output path | Topics 01--08 → `responses/unit_i/`; Topics 09--19 → `responses/unit_ii/` |
| 12 | Unicode math symbols | Use `\pi`, `\infty`, `\times`, `\cdot` -- never paste Unicode equivalents |
| 13 | Argand diagram missing labels | Label real axis, imaginary axis, and every plotted point |
