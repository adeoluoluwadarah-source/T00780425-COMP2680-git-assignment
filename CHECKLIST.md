# COMP2680 Assignment 7 (Git) — checklist

Prepared Thu Nov 12, 2026 (evening PST) from the assignment docx.
Source docx: ~/workspace/browser_downloads/sess-4025329799/browser-download-20261113T052415.263498754Z-0-COMP_2680_Assignment_7.docx

## Deadline — treat Moodle as binding
- **Tue Nov 17, 2026 at 12:59 AM PST (Moodle)** — i.e. Monday night, Nov 16.
- The docx says Nov 17 at 11:59 PM, almost a full day later. Work to 12:59 AM.
- Nothing submitted yet (checked Thu Nov 12, 9:24 PM PST).
- Submit one file: `T00780425-COMP2680-git-assignment1.pdf` or `.docx`
  (docx says "YourRollNo-COMP2680-git-assignment1.pdf/.docx" — use your student ID T00780425).
- Each step needs a screenshot + a 2–3 sentence description, including the live site.
- No marks / grading breakdown is listed in Moodle or the docx.

## What is already done here (Part A files)
- `index.html` (root), `css/styles.css`, `js/script.js` — built from the docx examples,
  plus one intro line: "Hi! I'm David, a TRU student in COMP2680…"
- Folder name matches the rule: `T00780425-COMP2680-git-assignment`
- NOT yet a git repo, NOT pushed to GitHub, NOT deployed — those steps are yours
  to run (they need your GitHub account), with the commands below.

## Part A — Repository setup
1. Copy this folder to where you keep coursework, or create the GitHub repo
   named `T00780425-COMP2680-git-assignment` first and clone it, then copy these files in.
2. `git init` (local) or clone, then:
   `git add .`
   `git commit -m "Initial commit: added HTML, CSS, and JS files"`
3. Screenshot: files + first commit.

## Part B — Branching (needs your bio — see below)
1. `git checkout -b feature-bio`
2. Add `aboutme.txt` with your hobbies/skills — **not written yet; see "Your two choices"**.
3. In this branch, add a paragraph to index.html about yourself.
4. `git add index.html aboutme.txt`
   `git commit -m "Added aboutme info and edited index.html"`
5. `git checkout main` and check `aboutme.txt` is NOT there.
6. Screenshots: branch creation, aboutme.txt, commit, back on main.

### Your two choices (needed before Part B/C)
- **Bio / hobbies for aboutme.txt:** the docx example is "I like coding, music, and web design."
  Known about you: volunteer coaching is on your resume. Your actual hobbies/skills
  are not on file — tell Muse what to put in, don't let it guess.
- **Favourite subject for the conflict (Part C):** pick two different topics, one for
  main and one for feature-bio, editing the SAME paragraph. E.g. main = one subject,
  feature-bio = a different subject. The resolved version keeps both ideas.

## Part C — Merging & conflict
1. On main: add a paragraph with your favourite subject/topic, commit:
   `git commit -m "Added favorite subject paragraph on main"`
2. On feature-bio: edit the SAME paragraph with a different topic, commit:
   `git commit -m "Edited favorite subject differently on feature-bio"`
3. `git checkout main` then `git merge feature-bio` — expect a conflict.
4. Open index.html, keep both ideas, save:
   `git add index.html`
   `git commit -m "Resolved merge conflict: preserved both topics"`
5. Screenshots: the conflict message, the resolved file, the merge commit.

## Part D — Deploy (GitHub Pages)
1. `git push origin main`
2. GitHub repo → Settings → Pages → Branch: main, Folder: / (root) → Save.
3. Wait a few minutes. Live URL will be:
   `https://<your-GitHub-username>.github.io/T00780425-COMP2680-git-assignment/`
4. Screenshot the live site and include it in the submission report.

## Submission report
- One Word/PDF, named `T00780425-COMP2680-git-assignment1.pdf` or `.docx`
- Screenshot + 2–3 sentences per step (A, B, C, D, including the live site).
- Muse can draft this report from your screenshots once the steps are done.
