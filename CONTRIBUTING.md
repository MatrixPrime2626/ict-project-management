# Contributing

Thanks for helping with the Digital Front Door prototype. Only the repository owner can change `main` directly. Everyone else proposes changes through a pull request.

## Workflow

1. **Fork** this repository (button at the top right on GitHub). Your fork is your own copy, so you can change anything in it.
2. **Clone your fork** and create a branch:
   ```bash
   git clone https://github.com/<your-username>/ict-project-management.git
   cd ict-project-management
   git switch -c short-description-of-change
   ```
   To start from an older version instead, branch from its tag: `git switch -c my-branch v2.0`.
3. **Edit `index.html`** and open it in a browser to check your change on desktop and mobile widths.
4. **Commit and push** to your fork:
   ```bash
   git add index.html
   git commit -m "Explain what changed and why (mention FR/NFR IDs if relevant)"
   git push -u origin short-description-of-change
   ```
5. **Open a pull request** into `MatrixPrime2626/ict-project-management` → `main`. Describe the change and add a screenshot if the UI changed.

The owner reviews the pull request and merges it, asks for changes, or closes it.

## Keeping your fork up to date

```bash
git remote add upstream https://github.com/MatrixPrime2626/ict-project-management.git
git fetch upstream --tags
git switch main
git merge upstream/main
git push
```

## Guidelines

- Keep the page a single self-contained `index.html`.
- Keep WCAG 2.2 AA: colour contrast, visible focus, labels on every field, keyboard access.
- One change per pull request makes review quicker.
