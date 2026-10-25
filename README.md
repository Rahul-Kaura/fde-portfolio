# Rahul Kaura · Portfolio

Personal site for my forward deployed engineering work: production AI deployments, technical reports and open-source field tools.

**Live:** https://fde-portfolio.onrender.com/

## What's on it

| View | Contents |
|---|---|
| Overview | Current assignment, highlights, an interactive map of where my work sits in an AI platform, featured reports |
| Deployments | Problem / shipped / result briefs for work at Uniphore and Empirik AI, filterable by company and area |
| Research | Three technical reports with citations to the published literature: declarative secret delivery on Kubernetes, structure-preserving document ingestion for RAG, and agentic incident response |
| Open source | [driftguard](https://github.com/Rahul-Kaura/driftguard) and [fieldrag](https://github.com/Rahul-Kaura/fieldrag) |
| Profile | Experience, education, stack, contact |

## How it's built

A single static `index.html` with no build step and no framework.

- Views switch client-side and are linkable by hash (`#research`, `#paper-incident`, ...).
- Light and dark themes follow the system setting through CSS custom properties.
- Layout is responsive down to phone width.
- The only external requests are Google Fonts.

## Run locally

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy

`render.yaml` defines a Render static site that publishes the repository root. Connect this repository in Render (New → Blueprint), or point an existing static site at it.
