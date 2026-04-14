# IEEE Double-Column Report Setup

## Project Structure

```
Report2/
├── main.tex                    # Main document file
├── sections/
│   ├── Introduction.tex
│   ├── LiteratureReview.tex
│   ├── ProblemStatement.tex
│   ├── Methodology.tex
│   ├── WorkDone.tex
│   └── Results.tex
└── README.md
```

## How to Use

1. **Edit the main template**: Update `main.tex` with:
   - Your project title
   - Author name(s)
   - Abstract and keywords
   - Bibliography entries

2. **Add content to sections**: Edit each `.tex` file in the `sections/` folder with your content:
   - Introduction.tex
   - LiteratureReview.tex
   - ProblemStatement.tex
   - Methodology.tex
   - WorkDone.tex
   - Results.tex

3. **Compile the document**: Use any LaTeX compiler (pdflatex, xelatex, etc.):
   ```bash
   pdflatex main.tex
   ```
   Or if using BibTeX for references:
   ```bash
   pdflatex main.tex
   bibtex main
   pdflatex main.tex
   pdflatex main.tex
   ```

## Features

- **IEEE Format**: Uses the `IEEEtran` document class with two-column layout
- **Modular Structure**: Each section is in a separate file for easy management
- **Pre-configured Packages**: Includes common packages for math, graphics, algorithms, etc.
- **Ready for References**: Bibliography section included and pre-formatted for IEEE style

## Customization

- Modify the `\documentclass` line in `main.tex` if you need different options
- Add more packages as needed
- Update the keywords and abstract sections
- Add figures, tables, and citations as appropriate

## Tips

- Use `\cite{ref1}` to cite references
- Use `\ref{fig:label}` and `\label{fig:label}` for figure references
- Use `\input{}` for including other files (already set up)
- Keep section files focused and avoid too much nesting
