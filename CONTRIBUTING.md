# Contributing to NEETI projects

Thanks for helping out! This guide applies to every NEETI repository unless that repo has its own.

## Never used Git before?

1. Install Git: https://git-scm.com/downloads (or use **GitHub Desktop**: https://desktop.github.com)
2. Set up your name and email:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "you@tecnico.ulisboa.pt"
   ```
3. Do GitHub's free "Introduction to GitHub" course: https://skills.github.com
4. Students: claim free GitHub Pro and other perks via the **GitHub Student Developer Pack** (education.github.com).

## The workflow (every change, every time)

```
issue  →  branch  →  commits  →  pull request  →  review  →  merge to main
```

1. **Pick or open an issue.** Assign yourself so others know you're on it.
2. **Get the latest code and create a branch** from `main`:
   ```bash
   git switch main
   git pull
   git switch -c feat/12-events-page      # type/issue-number-short-description
   ```
   Branch types: `feat/`, `fix/`, `content/`, `design/`, `docs/`, `chore/`
3. **Commit small, clear changes:**
   ```bash
   git add .
   git commit -m "Add events page layout"
   ```
4. **Push and open a pull request:**
   ```bash
   git push -u origin feat/12-events-page
   ```
   On GitHub, click **Compare & pull request**. Write `Closes #12` in the description so the issue closes automatically.
5. **Get one approval**, fix anything requested, then **Squash and merge**.
6. Delete the branch after merging.

## Rules

- **Never push directly to `main`.** (It's protected anyway.)
- **Never commit passwords, API keys or personal data** (e.g. member lists with phone numbers). If you do by accident, tell the tech lead immediately: removing it from history needs extra steps.
- Keep pull requests small. One feature or fix per PR.
- Be kind in reviews. Comment on the code, not the person.

## Need help?

Ask in the NEETI tech channel or open an issue with the `question` label.
