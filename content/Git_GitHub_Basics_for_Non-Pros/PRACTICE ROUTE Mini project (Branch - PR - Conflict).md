---
tags: [git-course, practice]
level: basics
estimated_time: 25-40min
---

# PRACTICE ROUTE Mini project (Branch - PR - Conflict)

> [!info] Goal
> You will run through a realistic mini workflow:
> **Branch → 2 commits → Push → PR → Create a conflict → Resolve it**

---

## Prerequisites
- [[TASK Clone (Get repo locally)]]
- [[TASK Create & switch branch]]

> [!tip]
> Best done in a **test repo** (so you won’t annoy your team).

---

## Step 1 — Clone a test repo
If you already have one, skip.

→ [[TASK Clone (Get repo locally)]]

---

## Step 2 — Create a branch
Create:
- `feature/practice-route`

→ [[TASK Create & switch branch]]

---

## Step 3 — Make two small commits
Pick a simple file like `README.md`.

### Commit #1
- Add a short section: “Practice Route”
- Commit message: `Add practice route section`

→ [[TASK Commit (Save a snapshot)]]

### Commit #2
- Add one more bullet list under that section
- Commit message: `Expand practice route details`

→ [[TASK Commit (Save a snapshot)]]

---

## Step 4 — Pull, then push
1) Pull:
→ [[TASK Pull (Get updates)]]

2) Push:
→ [[TASK Push (Upload your branch to GitHub)]]

---

## Step 5 — Open a PR
Create PR from `feature/practice-route` → `main`  
→ [[TASK Pull Request (Create PR & review)]]

---

## Step 6 — Create a conflict on purpose (safe method)
We want a conflict in the same file and same lines.

### Simulate “someone else changed main” (GitHub web editor)
1. Go to `README.md` on GitHub **on main**
2. Edit the same lines you changed (change wording)
3. Commit directly to `main` (in a test repo this is fine)

---

## Step 7 — Update your branch and hit the conflict
Back in your local `feature/practice-route` branch:

```bash
git pull
```

If the conflict doesn’t appear, run:
```bash
git pull origin main
```

Now you should see a conflict.

---

## Step 8 — Resolve conflict in VS Code
→ [[TASK Resolve conflicts (Merge conflicts)]]

After resolving:
```bash
git add .
git commit -m "Resolve merge conflict"
git push
```

---

## Step 9 — Verify the PR is clean again
- On GitHub PR: conflicts are gone
- Checks are green (if you have any)

---

## Done ✅
If you completed all steps, you can do the real workflow in a team repo.

---

### Navigation
Prev: [[00_START - Git in 60 Minutes (Roadmap)]]  
Next: [[CHEAT SHEET Git quick reference]]
