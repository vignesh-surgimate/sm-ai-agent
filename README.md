# Surgimate UI E2E Agent demo page

This folder is a standalone, public-safe static site inspired by the layout of the [QA Engineering Metrics & Quality Visibility page](https://vignesh-surgimate.github.io/qa-engineering-metrics-quality/). It presents the agent's purpose, architecture, evidence rules, matrix, and rollout readiness. The architecture section includes the supplied diagram and a link to its [Figma board](https://www.figma.com/board/hHXdDPUGFLjV7KVMRH1xsu/LangGraph-Playwright-Regression-Pipeline?node-id=2-146&t=LmIkBtIozqmaAj1S-1). The matrix calculator is illustrative; the page has no connection to a live agent or tenant.

## Preview locally

From this folder, run `python3 -m http.server 8000` and open `http://localhost:8000/`.

## Publish with GitHub Pages

Create a **separate repository containing only this folder's files**. Keep the agent's `.env`, SQLite databases, workbook, vendor access records, and run artifacts out of that repository. Push these files to its `main` branch, then choose **GitHub Actions** under repository **Settings → Pages → Build and deployment**. The included workflow publishes `index.html`, the diagram under `assets/`, and `.nojekyll` from the repository root. GitHub Pages sites can be public even when their source repository is private.

No GitHub repository was created or deployed by this task. Update the dated status copy in `index.html` after each verified milestone; never replace it with estimated pass counts.
