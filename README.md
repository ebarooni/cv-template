# LaTeX CV Template

A CV template written in LaTeX.

## Installation

### Install dependencies on macOS

1. Install Homebrew (if not already installed):
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```
   
2. Install MacTeX (no GUI version):
   ```bash
   brew install --cask mactex-no-gui
   ```
   
3. If using VS Code, install the LaTeX Workshop extension.

## Compilation

### Compile the full document

To generate the complete CV, run:

```bash
pdflatex main.tex
```

This will output a PDF containing all the defined pages.

### Compile individual pages

Files under the `pages/` directory can also be compiled separately:

```bash
pdflatex pages/<page-name>.tex
```

This is useful if you need to generate a specific page without compiling the entire document.

## Example Output

You can check out an already compiled version of the CV with placeholder values under the [`/example/main.pdf`](example/main.pdf) file.

## ⚠️ Limitations

- The hyperlinks in the resulting PDF file from compiling the `main.tex` do not work.
  - **Workaround:** To retain all links, compile each page separately and then merge them using an external tool (e.g. Mac Preview).
