# Contributing to Survival Data Analysis

Thanks for your interest in improving Survival Data Analysis. This guide covers how to report a problem, set up the project locally and propose a change.

## Reporting bugs and suggesting features

Open an [issue](https://github.com/Yvngval/Survival-data-analysis/issues) and include:

- what you expected and what happened instead
- the steps to reproduce it
- your environment (operating system, R version and package versions from `sessionInfo()`)

Security issues are the exception: report them privately as described in [SECURITY.md](SECURITY.md).

## Development setup

```bash
git clone https://github.com/Yvngval/Survival-data-analysis.git
cd Survival-data-analysis
Rscript -e 'install.packages(c("ggplot2", "FactoMineR", "cluster", "MASS"), repos = "https://cloud.r-project.org")'
Rscript Code/Code.R
```

## Proposing a change

1. Fork the repository and create a branch from `main`, for example `git checkout -b fix/node-groups`.
2. Keep each pull request focused on a single change.
3. Run `Rscript Code/Code.R` from the repository root and check that it completes and that the plots in `Rplots.pdf` still look right.
4. Write commit messages in the [Conventional Commits](https://www.conventionalcommits.org/) style, for example `fix: correct node count column name`.
5. Open a pull request that explains what changed and why.

## Code style

The script uses base R and ggplot2, with backtick-quoted column names in French and short comments above each step. Keep paths relative to the repository root.
