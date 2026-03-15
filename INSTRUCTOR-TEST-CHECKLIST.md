# Instructor Test Checklist (Simulate a Student Submission)

Use this to verify the workflow end-to-end before inviting students.

## A) Create a “test student” repo
1) Go to the template repo:
   https://github.com/thepusoproject/tpp-sari-sari-store
2) Click **Use this template**
3) Repo name suggestion:
   `tpp-sari-sari-store-test-student`
4) Set repo visibility:
   Public (to match current policy)

## B) Make a Module 00 submission (PR)
1) Clone the repo locally
2) Create branch:
   `module-00-setup`
3) Edit `STUDENT.md` (fill all fields)
4) Run:
   `python main.py`
5) Commit + push:
   - Commit message: `M00: add student profile`
6) Open PR:
   - Title: `Module 00 - Setup`
   - Description includes:
     - output screenshot/paste of `python main.py`
     - 2–3 sentences: what you installed / any issues

## C) Instructor grading test
1) Open the rubric:
   `grading/M00-rubric.md`
2) Score the PR and leave feedback
3) Confirm unlock rule:
   Pass >= 8/10 → Unlocked Module 01

## D) What “success” looks like
- PR exists with correct title
- Branch naming correct
- STUDENT.md is filled
- Evidence included
- Instructor can copy/paste feedback template quickly
