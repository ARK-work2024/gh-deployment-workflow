# gh-deployment-workflow
# GitHub Pages Deployment Workflow

This repository demonstrates how to automatically deploy a static website to GitHub Pages using GitHub Actions.

## How it works

- Any push to the `main` branch that **modifies `index.html`** triggers the workflow.
- The workflow builds and deploys the site to GitHub Pages.
- The deployed site is available at:https://ark-work2024.github.io/gh-deployment-workflow/

## Detailed explanation
A HTML file is created in a GitHub repository.
GitHub Pages hosts the website using a URL based on my GitHub username and repository name.

A CI/CD workflow is created inside .github/workflows/.
When changes are commiteed to index.html, GitHub spins up a temporary Ubuntu VM in the cloud, clones my repository into that VM, runs the deployment steps, uploads the site as an artifact, and publishes it to GitHub Pages.

Project URL: https://github.com/ARK-work2024/gh-deployment-workflow/blob/main/README.md
