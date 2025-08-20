## Resume

This repository contains my resume in LaTeX. Every time a push is made, the PDF is built and committed to the repository by GitHub Actions, and to my personal website.

### Local requirements

- [LaTeX](https://www.latex-project.org/get/)
- [Cursor](https://cursor.sh/) (recommended) or your favorite text editor

### How to use?

1. Clone the repository.

```bash
git clone https://github.com/Umutalb/resume.git
cd resume
```

2. Change the content of the `resume.tex` file with your own content.

3. To build the PDF locally, you can use the following command:

```bash
pdflatex resume.tex
```

4. To build the PDF with GitHub Actions, you can push the changes to the repository.

```bash
git add resume.tex
git commit -m "docs: update resume.tex"
git push
```

5. To push resume to your other repositories, you need to set `PAT_TOKEN` in your `resume` repository's action secrets section.

### Output

The generated PDF will be available as `Update_Umut_Resume.pdf` in the repository root. You can find the latest version [here](./Update_Umut_Resume.pdf). (You can change to your name from [action file](./.github/workflows/tex-to-pdf.yml))

### License

This project is licensed under the MIT License. See the [LICENSE.md](./LICENSE.md) file for details.
