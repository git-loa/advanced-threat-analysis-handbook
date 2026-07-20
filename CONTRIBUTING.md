
# Contributing to the Advanced Threat Analysis and Detection Engineering Handbook

Thank you for your interest in contributing to this handbook. This project is designed as a structured, modular reference for Cyber Threat Intelligence (CTI), threat hunting, detection engineering, SIEM operations, and Linux investigations. Contributions should follow the guidelines below to maintain consistency, clarity, and quality.

---

## Contribution Workflow

### 1. Fork the repository
Create your own fork of the repository and clone it locally.

### 2. Create a feature branch
Use a descriptive branch name:
```
git checkout -b add-new-detection-patterns
```

### 3. Add or modify LaTeX content
All handbook content lives in the `parts/` directory. Each file should be named descriptively:

Examples:
- `spl_fundamentals.tex`
- `linux_investigations.tex`
- `detection_playbooks.tex`
- `advanced_detection_patterns.tex`

Avoid generic names like `part1.tex`.

### 4. Update `main.tex` if needed
If you add a new section, include it in `main.tex` using:
```
\input{parts/your_filename.tex}
```

### 5. Build locally (optional)
If you want to preview the PDF locally:
```
pdflatex main.tex
```

GitHub Actions will automatically build the PDF on push, so local builds are optional.

### 6. Commit your changes
Use clear, descriptive commit messages:
```
git commit -m "Added new Linux persistence investigation section"
```

### 7. Push your branch
```
git push origin add-new-detection-patterns
```

### 8. Open a Pull Request
Describe:
- What you added or changed
- Why it improves the handbook
- Any references or sources used

---

## Style Guidelines

### Writing Style
- Use clear, professional language.
- Prefer long-form paragraphs over bullet-heavy sections.
- Avoid overly academic tone; prioritize operational clarity.
- Use consistent terminology (e.g., “detection engineering,” “threat hunting,” “CTI workflows”).

### LaTeX Formatting
- Use `\section{}` and `\subsection{}` — no chapters.
- Avoid custom macros unless necessary.
- Use `\lstlisting` for SPL, KQL, and command-line examples.
- Do not embed images unless essential.

### File Naming
Use descriptive, lowercase, underscore-separated names:
```
threat_hunting_fundamentals.tex
dashboard_design.tex
cti_workflows.tex
```

### Code Examples
Use fenced LaTeX listings:
```
\begin{lstlisting}
index=_internal | stats count by sourcetype
\end{lstlisting}
```

---

## PDF Builds

You do **not** need to commit PDFs.

GitHub Actions automatically:
- compiles `main.tex`
- generates `main.pdf`
- uploads it as an artifact

You can download the latest PDF from:
**GitHub → Actions → Latest run → Artifacts**

---

## Reporting Issues

If you find:
- typos
- unclear explanations
- incorrect SPL/KQL examples
- missing sections
- formatting problems

Please open an issue with:
- a clear description
- the affected file(s)
- suggested improvements

---

## License

By contributing, you agree that your contributions will be licensed under the repository’s MIT License.

---

Thank you for helping improve this handbook and supporting the CTI, threat hunting, and detection engineering community.