# GitHub Starter Tutorial

This tutorial is for getting one simple website online and using AI to build it.

No HTML, CSS, command-line, SSH, or Git experience is required.

## Quick start (what you're doing)

**Setup (one-time):**

1. **Create a repo** -- your own copy of this project on GitHub from the template.
2. **Run Initialize Tutorial Issues** -- generates a step-by-step checklist of GitHub Issues.

**Build your dashboard:**

1. **Install GitHub Desktop + clone** -- copies the repo to your computer.
2. **Open in an AI coding tool and build the dashboard** -- use opencode, Codex, or Claude Code to design your page locally with your own research artifacts.
3. **Commit and push** -- save and send your work to GitHub via GitHub Desktop.
4. **Publish with GitHub Pages** -- turn your repo into a live website.

You design and build before you publish. The first thing visitors see at your live URL is your real dashboard, not a blank template.

## What each tool does

- **GitHub** -- where your project lives online.
- **GitHub Desktop** -- copies the repo to your computer so AI coding tools can read and write your local files.
- **opencode / Codex / Claude Code** -- AI coding tools that read your folder, look at your research artifacts, and write the dashboard for you.
- **GitHub Pages** -- publishes your finished dashboard as a live website.
- **github.dev** -- optional browser-only editor for quick text edits. See `docs/addendums/addendum-f-github-dev-browser-edit.md`.

## What you'll finish

- A GitHub repository named `github-startup`.
- GitHub Desktop installed and connected to your repo.
- A local project folder at `Documents/GitHub/github-startup`.
- An AI coding tool opened to that same folder.
- A personal research dashboard, built with the AI, committed and pushed.
- A live GitHub Pages link.

## Setup

### Step 1: Create your repo

1. Create a GitHub account if you don't have one: https://github.com/signup
2. Open the original `github-starter-tutorial` repository (you're here now).
3. Click **Use this template**.
4. Choose **Create a new repository**.
5. Name it `github-startup`.
6. Make it **Public**.

### Step 2: Run Initialize Tutorial Issues

1. In your new `github-startup` repo, click the **Actions** tab.
2. If asked, enable workflows.
3. Click **Initialize Tutorial Issues** -> **Run workflow**.
4. Wait for it to finish (green checkmark).
5. Open the **Issues** tab -- the remaining steps are now issue checklists.

## Then follow the generated issues

- [ ] [Install GitHub Desktop and Clone Your Repo](docs/steps/02-install-github-desktop.md)
- [ ] [Open Your Folder in the AI Coding Tool and Build Your Dashboard](docs/steps/03-open-in-ai-tool-and-build.md)
- [ ] [Commit and Push from GitHub Desktop](docs/steps/04-commit-push-from-desktop.md)
- [ ] [Publish Your Dashboard with GitHub Pages](docs/steps/05-publish-with-github-pages.md)

## Optional addendums

- [Use opencode and the Free Vision Model](docs/addendums/addendum-e-opencode-and-deepseek.md) -- free path through Step 3 with vision support.
- [Open This Folder in Codex](docs/addendums/addendum-a-link-codex.md) -- paid, requires ChatGPT Pro.
- [Open This Folder in Claude Code](docs/addendums/addendum-b-link-claude-code.md) -- paid.
- [Edit Files in the Browser with github.dev](docs/addendums/addendum-f-github-dev-browser-edit.md) -- optional, for quick browser-only text edits.

See `docs/addendums/README.md` for the full list.

## Troubleshooting

### My GitHub Pages link is not updating

Pages can take a few minutes. Check: did you commit and push? On GitHub, does your repo show the new changes? In Settings > Pages, is the source set to `main` and `/ (root)`? Wait 2-5 minutes and refresh.

### I cloned the wrong folder

In GitHub Desktop, click **Repository > Show in Finder** or **Repository > Show in Explorer**. The folder should be `Documents/GitHub/github-startup`.

### My AI coding tool cannot see my files

Open the exact folder: `Documents/GitHub/github-startup`. You should see `index.html`, `style.css`, and `README.md`. If not, close and reopen the folder in your AI tool.

### opencode cannot read my reference images

You probably need to switch the model. See `docs/addendums/addendum-e-opencode-and-deepseek.md` for the model picker step.

### GitHub Desktop shows too many changed files

Make sure the current repository is `github-startup`, not your whole Documents folder.

### I edited files but do not know how to push

Open GitHub Desktop. Make sure the current repo is `github-startup`. Write a summary, click **Commit to main**, then click **Push origin**.

## Submission checklist

- [ ] Live GitHub Pages URL (paste into Canvas).

## Why this matters

GitHub is where your project lives. GitHub Desktop connects your local computer to your GitHub repo so AI coding tools can work with your files. The AI tool reads your research artifacts and writes the dashboard. GitHub Pages publishes the result. Once this loop works, you can use it for any web project.
