---
tags: [git-course, task]
level: basics
estimated_time: 6-10min
---

# TASK Create & switch branch

> [!info] Goal
> You work in your own branch (not on `main`).

---

## 1) Why?
A branch is your **safe work lane** so you don’t break the main line.

---

## 2) Do this now

### Option A: VS Code
1. Click the branch name bottom-left (e.g. `main`)
2. “Create new branch…”
3. Name it, e.g. `feature/login-fix`
4. VS Code switches automatically

### Option B: Terminal
```bash
git switch -c feature/login-fix
```

---

## 3) Check
```bash
git branch
```
Your current branch has `*`.

---

## 4) Common issues

> [!warning]- I’m back on `main`
> **Fix:**
> ```bash
> git switch feature/login-fix
> ```

> [!warning]- Branch names are messy
> **Tip:** use a scheme: `feature/...`, `bugfix/...`, `chore/...`

---

## 5) Mini exercise
- Create `feature/test-branch`
- Switch to `main`
- Switch back to `feature/test-branch`

---

## 6) Next step
→ [[TASK Commit (Save a snapshot)]]

---

### Navigation
Prev: [[TASK Clone (Get repo locally)]]  
Next: [[TASK Commit (Save a snapshot)]]
