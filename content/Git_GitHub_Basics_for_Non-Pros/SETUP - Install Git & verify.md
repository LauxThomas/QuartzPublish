---
tags: [git-course, setup]
level: basics
estimated_time: 10-15min
---
---
# SETUP - Install Git & verify

> [!info] Goal
> Git is installed, runs in your terminal, and you set your name/email.

---

## 1) Do this now

### Windows
- Install Git for Windows.
- Use “Git Bash” or the terminal inside VS Code.

### macOS
- Open Terminal → test `git --version`.
- If missing: install Xcode Command Line Tools (or use a package manager).

### Linux
- Install via your distro package manager.

> [!note]
> This course is tool-agnostic. The only requirement: `git` works.

---

## 2) Check: is Git available?
```bash
git --version
```

Expected: something like `git version x.y.z`

---

## 3) One-time config (name + email)
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Check:
```bash
git config --global --list
```

---

## 4) Optional: default branch name
Many teams use `main` (instead of `master`).
```bash
git config --global init.defaultBranch main
```

---

### Navigation
Prev: [[00_START - Git in 60 Minutes (Roadmap)]]  
Next: [[SETUP GitHub access (HTTPS vs SSH)]]
