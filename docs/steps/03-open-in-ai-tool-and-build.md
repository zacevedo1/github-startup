# Open Your Folder in the AI Coding Tool and Build Your Dashboard

## Goal

Open your local project folder in an AI coding tool and use it to build your personal research dashboard.

## Instructions

### Part A: Open the folder in your AI tool

Pick one tool. You only need one.

- **opencode** (free, includes a free vision-capable model). Install from https://opencode.ai/. After installing, open your project folder: `Documents/GitHub/github-startup`. See `docs/addendums/addendum-e-opencode-and-deepseek.md` for setup details, including how to switch to the free vision model so the AI can read your reference images.
- **Codex** (paid, requires ChatGPT Pro). Open https://chatgpt.com/codex/, then select `Documents/GitHub/github-startup`. See `docs/addendums/addendum-a-link-codex.md`.
- **Claude Code** (paid). Open Claude Code and select `Documents/GitHub/github-startup`. See `docs/addendums/addendum-b-link-claude-code.md`.

Once your AI tool is open, confirm it can see your files. Ask it to list the files in the folder. You should see `index.html`, `style.css`, and `README.md`.

### Part B: Drop in your research artifacts

Before you ask the AI to build the dashboard, drop your research files into the project folder. The AI will read them and use them.

- Markdown notes (`.md` files) from anywhere -- Milanote export, Notion export, Obsidian, plain text. Drop them in.
- Reference images (`.jpg`, `.png`, `.gif`, `.webp`). Drop them in.

If you do not have any markdown notes yet, that is okay -- the AI will interview you about your research instead. If you do not have reference images yet, that is also okay -- the dashboard does not require them.

### Part C: Build your dashboard

Paste this prompt into your AI tool. Do not paraphrase -- copy it as written.

```
Interview me about my research project. Ask me:
- What is the research question or topic I am exploring?
- What sources, notes, or artifacts have I collected so far?
- Do I have reference images that should be part of the dashboard?

Then read every markdown (.md) file in this folder. These are my research notes
and may come from Milanote, Notion, Obsidian, or plain text. Summarize what you
find.

Then look at every image file (.jpg, .png, .gif, .webp) in this folder. If you
can see them, describe what each one shows and how it might inform the dashboard's
visual direction. If you cannot see them, tell me you cannot and continue
without them.

Then propose a plan for turning index.html into a personal research dashboard
with these sections (you can rename or reorder if a better structure is
obvious from my materials):

- Research question (top of the page, framed clearly)
- Sources and notes (links and short summaries from the markdown files)
- Reference images (gallery or grid; every image needs alt text describing it)
- Notes and experiment log (chronological, dated entries)
- Workspace links (Milanote, Notion, Figma, GitHub - wherever the work lives)

Show me the plan before changing any files. After I approve, update index.html
and style.css. Keep the page accessible: semantic HTML, alt text on every image,
readable contrast. Do not add any JavaScript.
```

Go back and forth with the AI. It will show you a plan first. Review the plan, ask for changes, and approve when you are ready. Then it will edit the files.

### Part D: Preview your changes locally

1. In Finder or File Explorer, open `Documents/GitHub/github-startup`.
2. Double-click `index.html` -- it will open in your web browser.
3. You see your local changes here before they go live on GitHub Pages.

Iterate with the AI until you like what you see. The dashboard does not need to be perfect on the first try.

## Checklist

- [ ] My AI coding tool is open and can see `Documents/GitHub/github-startup`.
- [ ] My research artifacts (markdown notes + reference images) are in the project folder.
- [ ] I pasted the prompt verbatim and the AI showed me a plan before changing files.
- [ ] If I am using opencode on the free tier, I switched the model to the free vision-capable one in the picker.
- [ ] I previewed my changes locally by opening `index.html` in a browser.
- [ ] The dashboard reflects my research question, sources, and references.
