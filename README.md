# Data Analytics Portfolio: A Teaching Demo

A teaching example for graduate accounting data analytics students on building a personal analysis portfolio on GitHub.

> **Audience:** students in accounting data analytics.
> **Goal:** by the end, you can publish any analysis project to GitHub in a consistent, professional format.

## What is a README.md?

The `README.md` is the front page of a repository. GitHub renders it automatically. Employers, professors and teammates read it first, so it should answer in under a minute: *what is this, why does it matter, and how do I reproduce it?*

## Recommended README structure

| Section | Purpose |
|---|---|
| Title + one-line summary | What the project is, in plain language |
| Business question | The accounting/finance problem being answered (e.g. budget variance, fraud detection) |
| Data | Source, license, time period, key fields; never commit confidential data |
| Approach | Methods and tools (Python/R/Excel/SQL), key steps |
| Key findings | 3-5 bullets with numbers and one chart |
| How to reproduce | Environment setup and run commands |
| Repository structure | Folder tree with short descriptions |
| Limitations & next steps | Honest caveats |
| Author / contact | Name, LinkedIn, course |

A fill-in version lives in [`templates/project-template/README.md`](templates/project-template/README.md).

## Recommended project folder layout

```
project-name/
├── README.md          # front page (see above)
├── data/
│   ├── raw/           # original, never edited by hand
│   └── processed/     # cleaned data produced by code
├── notebooks/         # exploratory analysis
├── src/               # reusable scripts
├── reports/           # final write-ups, slides
├── figures/           # exported charts
├── requirements.txt   # dependencies
└── .gitignore
```

Naming rules: lowercase, hyphens for repos (`budget-variance-analysis`), numbered notebooks (`01_clean.ipynb`, `02_model.ipynb`).

## Publishing a project to GitHub

1. Copy `templates/project-template/` to a new folder and rename it.
2. Fill in the README.
3. Run:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: project structure and README"
   git branch -M main
   git remote add origin https://github.com/<you>/<project-name>.git
   git push -u origin main
   ```
4. Add a repo description and topics (e.g. `#budgeting`, `#accounting-analytics`) in the repo's "About" box.
5. Pin your best repositories on your GitHub profile.

Full checklist: [`docs/publishing-checklist.md`](docs/publishing-checklist.md).

## A repeatable "skill" for publishing future projects

[`.github/prompts/publish-project.prompt.md`](.github/prompts/publish-project.prompt.md) is a reusable prompt that asks an AI assistant to put any new analysis into this consistent format. Students can reuse and adapt it.

## Prompt engineering for portfolio building

See [`docs/prompt-engineering.md`](docs/prompt-engineering.md) for how to write effective prompts (role, context, task, constraints, output format) and examples.

## Confidentiality reminder

Accounting data is often sensitive. Use public or anonymized datasets only, and never commit credentials or client data.
