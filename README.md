# LSBU AI Foundry – Digital Front Door prototype

UX prototype for the **AI Foundry** at London South Bank University, built for the CSI_6_ICT *ICT Project Management in Practice* coursework (CW2).

LSBU staff use the Digital Front Door to submit process-automation requests. Digital Project Managers then score, triage and move those requests through the AI Foundry pipeline.

> This is a UX prototype, not a production system. Outside the Claude artifact it runs in **practice mode**: nothing is saved, and sample data is used so both the Requester and Digital Project Manager journeys can be walked through.

## Run it

Everything is in one file, `index.html` (layout, styles and JavaScript).

- **Quickest:** download the repo (green **Code** button → **Download ZIP**), unzip, and double-click `index.html`.
- **With git:**
  ```bash
  git clone https://github.com/MatrixPrime2626/ict-project-management.git
  cd ict-project-management
  ```
  then open `index.html` in a browser. Nothing needs installing.

## Versions

Each version is a commit on `main` with a tag, so you can view, download or branch from any of them.

| Tag | What it contains |
|-----|------------------|
| `v1.0` | Intake form with real-time validation, GDPR alert, governance banner and confirmation screen |
| `v2.0` | Saves submitted requests and adds a **My requests** view |
| `v3.0` | Aligned with Section 1 spec (FR1, FR2, FR6, NFR1, NFR2) and adds the Digital PM opportunity pipeline (FR3, FR4, NFR3, NFR5) |

### Start new work from an older version

```bash
git fetch --tags
git switch -c my-change-from-v1 v1.0   # new branch starting at v1
# edit index.html, then
git add index.html
git commit -m "Describe the change"
git push -u origin my-change-from-v1
```

On GitHub you can do the same without the command line: open the branch menu, choose the **Tags** tab, pick a version, then type a new branch name in the same menu to create a branch from it.

Compare two versions: `git diff v1.0 v2.0 -- index.html`, or on GitHub open `/compare/v1.0...v2.0`.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). In short: fork, work on a branch, and open a pull request. Changes reach `main` only after the repository owner reviews and merges them.
