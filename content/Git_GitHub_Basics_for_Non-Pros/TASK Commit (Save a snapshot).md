---
tags: [git-course, task]
level: basics
estimated_time: 8-10min
---

# TASK Commit (Save a snapshot)

> [!info] Goal
> You can commit changes cleanly (add → commit) and verify everything.

---

## 1) Why? (30 seconds)
A **commit** is a snapshot of your work. Make commits when you finish a small, meaningful step.

---

## 2) Do this now (step-by-step)

### Option A: VS Code (recommended)
1. Open Source Control (branch icon).
2. Review changed files.
3. Click **+** to Stage (or Stage All).
4. Write a short commit message.
5. Click **Commit**.

> [!tip] Good commit messages
> **Verb + object**, e.g.  
> - `Fix login crash`  
> - `Add onboarding text`  
> - `Refactor inventory UI`

---

### Option B: Terminal
1) Check status:
```bash
git status
```

2) Stage all:
```bash
git add .
```

3) Commit:
```bash
git commit -m "Add onboarding text"
```

> [!note] Stage a single file?
> ```bash
> git add path/to/file.ext
> ```

---

## 3) Check: am I done?
- [ ] `git status` shows **nothing to commit, working tree clean**
- [ ] `git log -1` shows your last commit (message looks right)

```bash
git status
git log -1
```

---

## 4) Common issues (If X → do Y)

> [!warning]- “nothing to commit” (but I changed something!)
> **Cause:** nothing changed or nothing was staged.  
> **Fix:**
> 1) Did you save the file?  
> 2) Check `git status`  
> 3) Then:
> ```bash
> git add .
> git commit -m "Your message"
> ```

> [!warning]- I staged too much (wrong files)
> **Fix (unstage):**
> ```bash
> git restore --staged .
> ```
> Then stage only what you want:
> ```bash
> git add path/to/file.ext
> ```

> [!warning]- My commit message is bad
> If you **haven’t pushed yet**:
> ```bash
> git commit --amend -m "Better message"
> ```

> [!warning]- I worked on `main` by accident
> **Easy fix (if not pushed yet):**
> ```bash
> git switch -c feature/my-feature
> ```
> Then continue normally.
> *(If already pushed and messy: see [[TROUBLESHOOTING If X happens, do Y]].)*

---

## 5) Mini exercise (1–2 minutes)
1. Change one small thing in a file.
2. Create a commit with a clean message.

Expected:
- [ ] `git log -1` shows the new commit
- [ ] Working tree is clean

---

## 6) Next step
→ [[TASK Pull (Get updates)]]
→ [[TASK Push (Upload your branch to GitHub)]]

---

### Navigation
Prev: [[TASK Create & switch branch]]  
Next: [[TASK Pull (Get updates)]]
