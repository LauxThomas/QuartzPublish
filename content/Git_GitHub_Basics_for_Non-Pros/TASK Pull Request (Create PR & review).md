---
tags: [git-course, task]
level: basics
estimated_time: 8-12min
---

# TASK Pull Request (Create PR & review)

> [!info] Goal
> You create a PR, describe it well, and prepare it for review.

---

## 1) Why?
PR = “Please merge my changes into `main`” + a place for review and checks.

---

## 2) Do this now (GitHub)
1. Open your repo on GitHub
2. Click “Compare & pull request” (or Pull requests → New pull request)
3. **Base**: `main` (or your team default)  
   **Compare**: your branch
4. Title: short and specific
5. Description template:

**What changed?**
- …

**Why?**
- …

**How to test?**

- …

---

## 3) Check
- PR shows the correct changes
- CI/checks (if any) are running/green
- Reviewer assigned (if needed)

---

## 4) Common issues

> [!warning]- PR targets the wrong base branch
> **Fix:** adjust Base/Compare in GitHub.

> [!warning]- PR is too big / too many topics
> **Fix:** smaller PRs get reviewed faster.

---

## 5) Mini exercise
- Create a PR with a clean description
- Review the “Files changed” tab

---

## 6) Next step
If conflicts appear:
→ [[TASK Resolve conflicts (Merge conflicts)]]

If all good:
→ [[CHEAT SHEET Git quick reference]]
→ [[PRACTICE ROUTE Mini project (Branch - PR - Conflict)]]

---

### Navigation
Prev: [[TASK Push (Upload your branch to GitHub)]]  
Next: [[TASK Resolve conflicts (Merge conflicts)]]
