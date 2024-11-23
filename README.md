# cv

Source for my LaTeX CV. The latest HTML version built from this repository is available [here](https://zeyu2001.github.io/cv/).

## Pre-commit Hooks

This repository uses the [pre-commit](https://pre-commit.com/) package manager to run hooks before each commit.

First install pre-commit:

```bash
pip install pre-commit
```

Then install the git hooks:

```bash
pre-commit install
```

The hook configuration is stored in [`.pre-commit-config.yaml`](.pre-commit-config.yaml). The specific hook being run is `latexindent`, and its behaviour can be configured in [`.latexindent.yaml`](.latexindent.yaml).

## VS Code Extension

It is also convenient to use the [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) extension for VS Code to build and preview the LaTeX files. Configure the `latexindent` command line arguments in the extension settings to match the configuration in `.pre-commit-config.yaml`.

## CI/CD

This repository uses GitHub Actions to deploy the HTML version to GitHub Pages. The workflow configuration is stored in [`.github/workflows/deploy-to-pages.yml`](.github/workflows/deploy-to-pages.yml). It uses [https://github.com/pdf2htmlEX/pdf2htmlEX](https://github.com/pdf2htmlEX/pdf2htmlEX) to convert the PDF to HTML.

## License

This repository is licensed under the MIT License. See [LICENSE](LICENSE) for more information.

**Note:** None of the information in this CV is particularly sensitive and it is in fact meant to be public. However, if you are considering forwarding my CV to a potential employer, please reach out to me first on LinkedIn or by email.
