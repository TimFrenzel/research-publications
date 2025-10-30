# Publishing White Papers to GitHub Pages

This repository automatically publishes white papers to GitHub Pages at:
**https://timfrenzel.github.io/research-publications/**

## How It Works

1. **Write your paper** in the `papers/YYYY/` folder structure
2. **Name your paper file** as `paper.md` or `paper.qmd`
3. **Add assets** to the `assets/` subfolder within your paper directory
4. **Push to GitHub** - automatic conversion to HTML happens via GitHub Actions
5. **Published!** Your paper appears on the website

## Folder Structure for Papers

```
papers/
└── 2025/
    └── 2025-11-ai-investment-management/
        ├── paper.qmd                    # Your white paper (markdown or Quarto)
        └── assets/                      # Optional: figures, charts, data
            ├── figure1.png
            └── chart2.png
```

## Writing Papers

### Option 1: Simple Markdown (`.md`)
Write your paper in standard markdown format:

```markdown
---
title: "AI in Investment Management"
author: "Tim Frenzel"
date: "2025-11-01"
---

## Executive Summary

Your content here...
```

### Option 2: Quarto Markdown (`.qmd`)
Use Quarto features for enhanced formatting:

```markdown
---
title: "AI in Investment Management"
author: "Tim Frenzel"
date: "2025-11-01"
format:
  html:
    toc: true
    code-fold: true
bibliography: references.bib
---

::: callout-note
## Executive Summary
- Key point 1
- Key point 2
:::

## Introduction

Your content here with citations [@source2023].
```

## Local Preview (Optional)

To preview how your paper will look before pushing:

### Install Quarto
```bash
# Download from https://quarto.org/docs/get-started/
# Or use package manager:
# Windows: choco install quarto
# Mac: brew install quarto
```

### Render Paper Locally
```bash
cd papers/2025/2025-11-your-paper-name/
quarto render paper.qmd --to html
```

This creates `paper.html` in the same directory for preview.

## Manual Conversion (Alternative)

If you prefer to convert papers manually instead of using the automated workflow:

```bash
# Navigate to your paper directory
cd papers/2025/2025-11-your-paper-name/

# Convert to HTML
quarto render paper.qmd --to html --output ../../../docs/papers/2025/your-paper-name.html

# Copy assets
cp -r assets/ ../../../docs/papers/2025/your-paper-name_assets/

# Commit and push
git add docs/
git commit -m "Publish: Your Paper Title"
git push
```

## Updating the Index Page

After publishing a paper, update `docs/index.html` to add your paper to the publications list:

```html
<li class="paper-item">
    <div class="paper-title">
        <a href="papers/2025/2025-11-your-paper.html">Your Paper Title</a>
    </div>
    <div class="paper-meta">November 2025 • 3-page white paper</div>
    <div class="paper-description">
        Brief description of your paper...
    </div>
    <div class="paper-links">
        <a href="papers/2025/2025-11-your-paper.html">Read Paper</a>
        <a href="https://github.com/TimFrenzel/research-publications/blob/main/papers/2025/2025-11-your-paper/paper.md">View Source</a>
    </div>
</li>
```

## GitHub Pages Configuration

To enable GitHub Pages for this repository:

1. Go to **Settings** → **Pages**
2. Under **Source**, select: **Deploy from a branch**
3. Under **Branch**, select: **main** branch and **/docs** folder
4. Click **Save**

Your site will be available at: `https://timfrenzel.github.io/research-publications/`

## Troubleshooting

### Papers not converting
- Check that your paper is named `paper.md` or `paper.qmd`
- Verify the YAML frontmatter is valid
- Check GitHub Actions logs for errors

### Images not displaying
- Ensure images are in the `assets/` subfolder
- Use relative paths: `![Description](assets/figure1.png)`
- Check file names match exactly (case-sensitive)

### Citations not working
- Add a `references.bib` file in your paper directory
- Include `bibliography: references.bib` in YAML frontmatter
- Use citation syntax: `[@author2023]`

## Workflow Summary

```
┌─────────────────┐
│  Write paper    │
│  (paper.qmd)    │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│  git push       │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ GitHub Actions  │
│ converts to HTML│
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Published on    │
│ GitHub Pages    │
└─────────────────┘
```

## Tips

- **Keep it simple**: Start with markdown (`.md`) format
- **Test locally**: Use Quarto to preview before pushing
- **Organize assets**: Keep all figures in the `assets/` folder
- **Use templates**: Copy `WHITEPAPER_TEMPLATE.md` for consistency
- **Version control**: Each paper is self-contained for easy management

