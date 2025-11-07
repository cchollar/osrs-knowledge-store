# Contributing to the OSRS Knowledge Store (GitHub + Obsidian Publish)

Thanks for your interest in improving this store of OSRS knowledge! This repository backs an Obsidian vault that’s published via **Obsidian Publish**. Contributions are welcome through GitHub Pull Requests (PRs).

> **Live site:** https://publish.obsidian.md/osrs-knowledge-store/  
> **Repo:** https://github.com/cchollar/osrs-knowledge-store

---

## TL;DR — Two Ways to Contribute

**Option A — Fork & PR (recommended for most):**
1. Click **Fork** on GitHub.
2. Clone your fork (or use GitHub Desktop / the web editor).
3. Create a branch, make changes, push, and open a **Pull Request** to this repo’s `main`.

**Option B — Ask for Contributor Access (for frequent collaborators):**
1. Open a **GitHub Issue** titled “Access request”.
2. Include your **GitHub username** and a short note on what you’d like to help with.
3. After approval, create a branch in this repo and open PRs as usual.

> Not ready to use Git yet? You can also open an **Issue** with your suggested edits or attach a Markdown file—maintainers can turn it into a PR.

---

## Git in 5 Minutes (for the uninitiated)

- **Git** is a version control system: it tracks changes to files over time so multiple people can work safely.
- **Repository (repo):** a folder tracked by Git (this vault lives in a GitHub repo).
- **Commit:** a saved checkpoint of your changes with a message describing *what* and *why*.
- **Branch:** a parallel line of work (like a copy of the project where you experiment). Create one per change.
- **Fork:** your own copy of the repo under your GitHub account. Edit your fork, then propose changes back.
- **Pull Request (PR):** a request to merge your branch/fork into the main project after review.

**Mental model:** Work in your own space (a **branch** or **fork**), **commit** changes, and open a **PR** so maintainers can review and merge.

---

## Local Setup (Either Path)

**Requirements**
- [Obsidian](https://obsidian.md/)
- Git tooling of your choice:
  - **Easiest (no terminal):** [GitHub Desktop](https://desktop.github.com/)
  - **In the browser:** Click a file → ✏️ to edit, or press `.` in the repo to open the web editor
  - **Terminal (optional):** Install [Git](https://git-scm.com/)

**Steps**
1. **Get the files:**
   - **Fork route:** Fork → **Code** → copy URL → clone your fork in GitHub Desktop or terminal.
   - **Contributor route:** Once added, clone the main repo directly.
2. **Open in Obsidian:** Obsidian → **Open folder as vault** → select the cloned folder.
3. **Suggested Obsidian settings (optional but helpful):**
   - **Default attachment location:** `assets/`
   - **New link format:** Relative path

---

## Option A — Fork & Pull Request (Step-by-Step)

**Using GitHub Desktop (no terminal):**
1. On the repo page, click **Fork**.
2. In GitHub Desktop: **File → Clone repository…** → choose your fork.
3. **Branch → New Branch…** → name it like `feat/topic-shortdesc`.
4. Open the folder in **Obsidian**, make edits, save.
5. In GitHub Desktop: **Commit** your changes with a clear message.
6. Click **Push origin**.
7. Click **Create Pull Request** (Desktop will open the PR dialog on GitHub).
8. Fill out the PR form (see “PR Checklist” below) and submit.

**Using Terminal (optional):**
```bash
# 1) Clone your fork
git clone https://github.com/cchollar/osrs-knowledge-store.git
cd osrs-knowledge-store

# 2) Create a branch
git checkout -b feat/topic-shortdesc

# 3) Make edits in Obsidian, then stage & commit
git add .
git commit -m "feat: add/update <short description>"

# 4) Push and open a PR
git push -u origin feat/topic-shortdesc
# Then open a PR on GitHub from your branch to the main repo's `main`
```

**Keeping your fork in sync (if needed):**
```bash
git remote add upstream https://github.com/<owner>/<vault>.git
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```

---

## Option B — Request Contributor Access

1. Open a **new Issue** titled “Access request”.
2. Include:
   - Your **GitHub username**
   - What you plan to contribute (ongoing docs, regular fixes, etc.)
3. After approval, you’ll be invited as a collaborator.
4. Create a feature branch in this repo and open PRs as normal:
   ```bash
   git checkout -b feat/topic-shortdesc
   # (edit files)
   git add .
   git commit -m "feat: <summary>"
   git push -u origin feat/topic-shortdesc
   ```
> Even with write access, please use **branches + PRs** (don’t push directly to `main`).

---

## What to Edit (Obsidian Notes)

- Add or update Markdown notes anywhere appropriate in the repo’s folder structure.
- Place images/attachments in `attachments/` (or a subfolder).

**Before you commit, please double-check:**
- No secrets, tokens, or personal data.
- Links resolve; images live in `attachments/` and use relative paths.

---

## PR Checklist (copy into your PR description)

- [ ] Changes view correctly in Obsidian
- [ ] Internal links resolve; external links are valid
- [ ] Any new images are in `attachments/` and linked relatively
- [ ] No secrets/PII are included

---

## Reviews & Publishing

- A maintainer will review your PR for clarity and correctness.
- After merge, changes are included whenever Cam has time to publish the new pages.
- If something should **not** go live yet, mention it in the PR (or mark it as a draft page if the repo uses frontmatter flags).

---
## Questions?

- Open a **GitHub Issue** with your question or idea.
- Or tag a maintainer in your PR.
- Maintainer: Cameron C — `autodidaktos` on Discord
