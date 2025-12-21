---
tags: [git-course, troubleshooting]
level: basics
estimated_time: 10-20min
---

# TROUBLESHOOTING If X happens, do Y

> [!info] Goal
> Fast fixes without panic.

---

## Auth & access

> [!warning] Permission denied (publickey)
→ Check SSH setup: [[SETUP GitHub access (HTTPS vs SSH)]]

> [!warning] Repository not found
→ Wrong URL / missing permissions / wrong repo.

---

## Commit & stage

> [!warning] nothing to commit, working tree clean
→ No changes or nothing staged.  
→ See: [[TASK Commit (Save a snapshot)]]

> [!warning] I staged too much
```bash
git restore --staged .
```
Then stage only what you want.

---

## Pull/Push problems

> [!warning] rejected (non-fast-forward)
1) Pull:
```bash
git pull
```
2) If conflict:
→ [[TASK Resolve conflicts (Merge conflicts)]]
3) Then push:
→ [[TASK Push (Upload your branch to GitHub)]]

> [!warning] Your local changes would be overwritten by merge
→ Commit first:
→ [[TASK Commit (Save a snapshot)]]

---

## “I worked on main…”
If not pushed yet:
```bash
git switch -c feature/my-feature
```
Then continue normally (push + PR).

If already pushed:
- open a PR or coordinate with your team (depends on context)

---

## If everything is on fire (emergency plan)
1) copy `git status`
2) what were you trying to do? (pull/push/merge)
3) what is the exact error message?
4) solve step by step (never run random commands)

---

### Navigation
Prev: [[TASK Resolve conflicts (Merge conflicts)]]  
Next: [[CHEAT SHEET Git quick reference]]
