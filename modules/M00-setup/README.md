# Module 00 — Setup + GitHub PR workflow (Taglish)

## Goal
By the end of this module, kaya mo na:
- i-run ang project locally
- gumawa ng branch
- mag-commit
- mag-push
- gumawa ng **Pull Request** for submission

## Required installs
- Python 3
- Git
- VS Code (recommended)

## Student workflow (standard)
1. Create your repo from the template `tpp-sari-sari-store`.
2. Clone your repo:
   - `git clone <your-repo-url>`
3. Create a branch:
   - `git checkout -b module-00-setup`
4. Run:
   - `python main.py` (or `python3 main.py`)
5. Make a small change (required):
   - edit `STUDENT.md` and fill your name + goals
6. Commit + push:
   - `git add STUDENT.md`
   - `git commit -m "M00: add student profile"`
   - `git push -u origin module-00-setup`
7. Open a PR:
   - Title: `Module 00 - Setup`
   - Description: what you installed + screenshot of successful run

## Submission requirements (PR)
- PR title matches
- `STUDENT.md` filled
- Screenshot in PR description

## Rubric (10 pts)
- (4) PR created correctly + title
- (3) `STUDENT.md` complete
- (3) Evidence screenshot + can run `main.py`
