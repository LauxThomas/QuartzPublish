---
tags: [git-course, cheatsheet]
level: basics
estimated_time: 5-8min
---

# CHEAT SHEET Git quick reference

> [!info] The 6 most important commands
```bash
git status
git add .
git commit -m "..."
git pull
git push
git log -1
```

---

## Standard workflow (short)
```bash
git pull
# work...
git add .
git commit -m "Describe change"
git push
```

---

## Branching
Create a new branch:
```bash
git switch -c feature/name
```

Switch branches:
```bash
git switch feature/name
```

---

## Unstage (if you staged too much)
```bash
git restore --staged .
```

---

## Improve last commit message (only if not pushed)
```bash
git commit --amend -m "Better message"
```

---

## Conflicts (short version)
1) open file
2) choose the correct resolution (VS Code buttons)
3) save
4) add + commit:
```bash
git add .
git commit -m "Resolve merge conflict"
```

---

## 3 rules that prevent 90% of stress
1) **Pull before push**
2) **Small commits**
3) **Don’t work on main**

---

### Navigation
Prev: [[TROUBLESHOOTING If X happens, do Y]]  
Next: [[PRACTICE ROUTE Mini project (Branch - PR - Conflict)]]
