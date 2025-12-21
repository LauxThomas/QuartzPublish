---
tags: [git-course, task]
level: basics
estimated_time: 6-10min
---

# TASK Push (Upload your branch to GitHub)

> [!info] Goal
> Your commits are visible on GitHub (in your branch).

---

## 1) Why?
“Push” uploads your local commits to the remote (GitHub).  
Only then you can open a Pull Request.

---

## 2) Do this now

### Option A: VS Code
1. Open Source Control
2. Click “Publish Branch” / “Push” (VS Code often suggests it)

### Option B: Terminal
First push for a new branch:
```bash
git push -u origin <branchname>
```

After that:
```bash
git push
```

---

## 3) Check
- On GitHub: your branch exists
- VS Code shows no pending arrows (0↑ 0↓)

Optional:
```bash
git status
```

---

## 4) Common issues

> [!warning]- rejected (non-fast-forward)
> **Cause:** remote has new commits.  
> **Fix:** pull first, resolve conflicts if needed:
> → [[TASK Pull (Get updates)]]
> → [[TASK Resolve conflicts (Merge conflicts)]]

> [!warning]- Auth/permission error
> **Fix:** check setup:
> → [[SETUP GitHub access (HTTPS vs SSH)]]

---

## 5) Mini exercise
- Push your branch
- Verify your commit appears on GitHub

---

## 6) Next step
→ [[TASK Pull Request (Create PR & review)]]

---

### Navigation
Prev: [[TASK Pull (Get updates)]]  
Next: [[TASK Pull Request (Create PR & review)]]
