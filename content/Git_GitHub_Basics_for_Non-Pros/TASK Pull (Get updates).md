---
tags: [git-course, task]
level: basics
estimated_time: 6-10min
---

# TASK Pull (Get updates)

> [!info] Goal
> You pull new changes from the remote before you continue or push.

---

## 1) Why?
“Pull” = fetch updates + integrate them.  
This reduces conflicts and “my local copy is outdated” problems.

---

## 2) Do this now

### Option A: VS Code
1. Open Source Control
2. “…” menu → **Pull**
3. If conflicts appear → [[TASK Resolve conflicts (Merge conflicts)]]

### Option B: Terminal
```bash
git pull
```

---

## 3) Check
```bash
git status
```
Expected: no fatal errors, ideally clean.

---

## 4) Common issues

> [!warning]- Merge conflict during pull
> Totally normal.  
> → [[TASK Resolve conflicts (Merge conflicts)]]

> [!warning]- “Your local changes would be overwritten”
> **Cause:** you have uncommitted changes.  
> **Fix:** commit first → [[TASK Commit (Save a snapshot)]]

---

## 5) Mini exercise
- Run `pull` (even if nothing comes)
- “Already up to date” is fine.

---

## 6) Next step
→ [[TASK Push (Upload your branch to GitHub)]]

---

### Navigation
Prev: [[TASK Commit (Save a snapshot)]]  
Next: [[TASK Push (Upload your branch to GitHub)]]
