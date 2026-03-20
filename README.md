# Carleton Lab Manual

A [Quarto book](https://quarto.org/docs/books/) serving as the onboarding and reference manual for the Carleton Research Group at UC Berkeley's [Department of Agricultural & Resource Economics (ARE)](https://are.berkeley.edu/) and [Center for Effective Global Action (CEGA)](https://cega.berkeley.edu/).

The published book is available at the lab's GitHub Pages site.

## Contents

| Part | Chapters |
|---|---|
| **About the Lab** | Mission, Values & Culture, Code of Conduct |
| **Working in the Lab** | Expectations, Onboarding, Offboarding |
| **Research Workflow** | Project Management, Data & Code Practices, Tools & Platforms, Writing & Publication |
| **High Performance Computing** | HPC Overview, Storage & Data, Compute Resources, Remote SSH, Containers |
| **Administrative** | Housekeeping |

## Local development

Requires [Quarto](https://quarto.org/docs/get-started/) ≥ 1.4.

Preview the book locally with live reload:

```bash
quarto preview
```

To do a full render without serving:

```bash
quarto render
```

Output is written to `_book/`. This directory is not committed — the live site is built and deployed automatically via GitHub Actions on every merge to `main`.

## Contributing

### Workflow

1. **Create a branch** off `main` for your changes:
   ```bash
   git checkout -b your-branch-name
   ```

2. **Edit content** — chapters are `.qmd` files in [chapters/](chapters/). Book structure and metadata are defined in [_quarto.yml](_quarto.yml).

3. **Preview locally** to verify your changes render correctly:
   ```bash
   quarto preview
   ```

4. **Open a pull request** against `main`. Describe what you changed and why.

5. **After review and approval**, merge the PR. The GitHub Actions workflow will automatically build and deploy the updated book to GitHub Pages.

> Note: do not commit the `_book/` directory. The deployment workflow handles rendering and publishing.

### Adding or reordering chapters

- New `.qmd` files go in [chapters/](chapters/).
- Register them in the `chapters:` list in [_quarto.yml](_quarto.yml) to include them in the book.
- Chapter order in the sidebar matches the order in `_quarto.yml`.

## Authors

- **Cullen Molitor** — Data Scientist, CEGA, UC Berkeley
- **Tamma Carleton** — Principal Investigator, ARE, UC Berkeley
