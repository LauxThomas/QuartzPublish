---
tags: [git-course, task]
level: basics
estimated_time: 6-10min
---

# TASK Clone (Get repo locally)

> [!info] Goal
> You have the GitHub repo on your computer and can open it.

---

## 1) Why?
“Clone” downloads the project as a folder **with full history**.

---

## 2) Do this now

### Option A: VS Code
1. On GitHub: open repo → “Code” → copy URL (HTTPS or SSH).
2. In VS Code: `Ctrl/Cmd + Shift + P` → **Git: Clone**
3. Paste URL → choose destination folder
4. Click “Open”

### Option B: Terminal
```bash
git clone <REPO-URL>
cd <repo-folder>
```

---

## 3) Check
```bash
git status
```
Expected: you’re inside a repo (no fatal error).

---

## 4) Common issues

> [!warning]- Repository not found / no access
> **Cause:** wrong URL or missing permissions.  
> **Fix:** verify URL / ask for access.

> [!warning]- Permission denied (publickey)
> **Cause:** SSH key missing / not added to GitHub.  
> **Fix:** [[SETUP GitHub access (HTTPS vs SSH)]]

---

## 5) Mini exercise
- Open the repo folder
- Find the README file

---

## 6) Next step
→ [[TASK Create & switch branch]]

---

### Navigation
Prev: [[SETUP VS Code setup (recommended)]]  
Next: [[TASK Create & switch branch]]
