---
tags: [git-course, setup]
level: basics
estimated_time: 10-20min
---

# SETUP GitHub access (HTTPS vs SSH)

> [!info] Goal
> You can authenticate to GitHub without pain.

---

## Which option should I pick?
### Option A: HTTPS (easiest)
✅ Quick setup  
✅ Great for beginners  
⚠️ You may need a token/credential flow depending on your system

### Option B: SSH (best for frequent use)
✅ Very convenient once set up  
⚠️ Takes a bit longer (create key, add to GitHub)

> [!tip]
> If you want to start right now: **HTTPS**.  
> If you work with Git often: **SSH** is worth it.

---

## 1) Use HTTPS
When cloning, use the URL that starts with `https://`.

If you’re asked for credentials during push/pull:
- Use your GitHub login/token (system-dependent)
- VS Code often helps automatically

---

## 2) Use SSH (short setup)
### A) Check if you already have a key
```bash
ls -al ~/.ssh
```

### B) Create a key (if you don’t have one)
```bash
ssh-keygen -t ed25519 -C "your.email@example.com"
```

### C) Start agent + add key
```bash
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
```

### D) Copy the public key
```bash
cat ~/.ssh/id_ed25519.pub
```
Add it in GitHub: Settings → SSH and GPG keys → New SSH key

### E) Test
```bash
ssh -T git@github.com
```

---

## Check: which URL type am I using?
- HTTPS: `https://github.com/...`
- SSH: `git@github.com:...`

---

### Navigation
Prev: [[SETUP - Install Git & verify]]  
Next: [[SETUP VS Code setup (recommended)]]
