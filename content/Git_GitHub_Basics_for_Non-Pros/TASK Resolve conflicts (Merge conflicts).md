---
tags: [git-course, task]
level: basics
estimated_time: 12-15min
---

# TASK Resolve conflicts (Merge conflicts)

> [!info] Goal
> You can resolve a simple conflict in VS Code and finish with a clean commit.

---

## 1) Why?
A conflict means: **two edits don’t merge automatically**.  
This is normal in team work.

---

## 2) How to spot conflicts
- `git pull` or a merge/PR shows “conflict”
- VS Code marks files as “Merge Changes”
- GitHub PR shows “This branch has conflicts”

---

## 3) Do this now (VS Code: beginner-friendly)
1. Open the conflicted file in VS Code
2. You’ll see markers like:
   `<<<<<<<`, `=======`, `>>>>>>>`
3. VS Code offers buttons:
   - **Accept Current Change**
   - **Accept Incoming Change**
   - **Accept Both Changes**
   - **Compare Changes**
4. Pick the correct option (or merge manually)
5. **Save**
6. Then stage + commit:

```bash
git add .
git commit -m "Resolve merge conflict"
```

---

## 4) Check
```bash
git status
```
Expected: clean.

Optional:
```bash
git log -1
```

---

## 5) Common issues

> [!warning]- I removed markers but the content is wrong
> **Fix:** read the file carefully and ensure the **meaning** is correct, not just the markers.

> [!warning]- More conflicts keep appearing
> **Fix:** go file by file, step by step.  
> If it escalates: [[TROUBLESHOOTING If X happens, do Y]]

---

## 6) Mini exercise (safe)
If you want to practice without annoying your team:
- create a conflict in a test repo (edit the same line in two branches)
- try to merge
- resolve the conflict

---

## 7) Next step
→ [[TASK Push (Upload your branch to GitHub)]]
→ [[TROUBLESHOOTING If X happens, do Y]]

---

### Navigation
Prev: [[TASK Pull Request (Create PR & review)]]  
Next: [[TROUBLESHOOTING If X happens, do Y]]
