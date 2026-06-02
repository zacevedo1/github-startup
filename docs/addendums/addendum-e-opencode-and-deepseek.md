# Optional: Use opencode and the Free Vision Model

Use this addendum if you do not have Codex or Claude Code and want a free path through Step 3 (the AI dashboard build).

## When to use this

- You do not have a paid AI coding subscription.
- You want the AI to read your reference images, not just your text notes.
- You want a free coding tool that runs on your computer.

## Instructions

### Part A: Install opencode

1. Go to https://opencode.ai/.
2. Follow the install instructions for your operating system. (The opencode site keeps its install steps up to date; this addendum does not duplicate them so they cannot go stale.)
3. Open opencode after installing.

### Part B: Open your project folder

1. In opencode, open your project folder: `Documents/GitHub/github-startup`.
2. Confirm opencode can see your files. Ask it to list the files. You should see `index.html`, `style.css`, `README.md`, and any research artifacts you dropped in.

### Part C: Switch to the free vision model

This is the step that lets opencode read your reference images, not just text.

1. In opencode, open the model picker.
2. Look for the free vision-capable model. As of 2026-05-27, it appears in the picker as **DeepSeek V4 Flash Free** (alongside other free models like `Big Pickle` and `Nemotron 3 Super Free`).
3. Select **DeepSeek V4 Flash Free**.

If you do not see DeepSeek V4 Flash Free in your picker, opencode may have renamed or rotated their free models. Pick whatever the picker labels as free and vision-capable. If you cannot tell, ask in office hours.

### Part D: Confirm vision works

1. Drop one reference image (`.jpg` or `.png`) into your project folder.
2. In opencode, ask: `Describe the image file in this folder. What is in it?`
3. You should get a real description of the image, not "I cannot see images."

If vision is not working on the free tier on your specific day, you have two options:
- Paste a written description of each reference image into a markdown file (e.g., `references-described.md`) and tell the AI to use that instead.
- Come to office hours and we will use a paid tool together for the vision part.

## Tool note

Opencode's free-tier model lineup can change. The label "DeepSeek V4 Flash Free" is what the picker shows at the time this addendum was written. If it disappears, look for any free, vision-capable model in the picker.

## Checklist

- [ ] opencode is installed and open.
- [ ] opencode can see `Documents/GitHub/github-startup` and its files.
- [ ] I switched the model to a free vision-capable one (e.g., DeepSeek V4 Flash Free).
- [ ] I confirmed vision works by asking the AI to describe a reference image.
