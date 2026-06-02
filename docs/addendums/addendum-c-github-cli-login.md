# Addendum C: GitHub CLI / Terminal Authentication

This addendum is advanced and optional.

The required tutorial does not use Terminal, Git commands, SSH keys, or GitHub CLI. GitHub Desktop handles the beginner path.

Use this only if your instructor asks, or if you are using a tool that specifically needs GitHub CLI authentication.

## Goal

Authenticate Terminal-based tools with your GitHub account.

## Instructions

1. Open your terminal app.
2. Run:

   ```bash
   gh auth login
   ```

3. When prompted, choose:

   - Account: `GitHub.com`
   - Protocol for Git operations: `HTTPS`
   - Authenticate Git with GitHub credentials: `Yes`
   - Authentication method: `Login with a web browser`

4. Copy the one-time code shown in the terminal.
5. Open <https://github.com/login/device>.
6. Paste the code and authorize.
7. Verify with:

   ```bash
   gh auth status -h github.com
   ```

## Checklist

- [ ] I understand this is not required for the beginner path.
- [ ] I completed `gh auth login`, if needed.
- [ ] GitHub CLI shows that I am logged in, if needed.
