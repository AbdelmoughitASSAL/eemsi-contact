# 🚀 Easy Deployment Guide

Deploy your HTML site to GitHub Pages in 5 minutes!

---

## Step 1: Create a GitHub Repository

1. Go to **github.com**
2. Click the **+** icon (top-right) → **New repository**
3. Fill in:
   - **Repository name:** `my-awesome-site` (or any name)
   - **Description:** (optional)
   - Select **Public** (so it's visible)
   - **DO NOT** check "Initialize with README"
4. Click **Create repository**

**You'll see a screen with commands. Copy the repository URL** (looks like `https://github.com/username/my-awesome-site.git`)

---

## Step 2: Initialize Git & Push Your Code (One Time Only)

Open your terminal and run these commands:

```bash
# Navigate to your project folder
cd your-project-folder

# Initialize git
git init

# Add all files
git add .

# Create first commit
git commit -m "Initial commit"

# Connect to GitHub (replace with YOUR repo URL)
git remote add origin https://github.com/YOUR_USERNAME/your-repo-name.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**That's it! Your code is now on GitHub.**

---

## Step 3: Enable GitHub Pages (One Time Only)

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Click **Pages** (left sidebar)
4. Under "Source":
   - Select **Deploy from a branch**
   - Choose **main** branch
   - Choose **/ (root)**
5. Click **Save**

**Wait 1-2 minutes...**

Your site will be live at:
```
https://your-username.github.io/your-repo-name/
```

---

## Step 4: Update Your Site (After First Deploy)

When you make changes to your code:

```bash
# Stage your changes
git add .

# Commit with a message
git commit -m "Update: describe what changed"

# Push to GitHub
git push
```

**That's it! Your site updates automatically within seconds.** ✨

---

## Quick Reference

### First time setup:
```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/username/repo.git
git branch -M main
git push -u origin main
```

### Every time you update:
```bash
git add .
git commit -m "Your message"
git push
```

---

## Common Issues

### "Changes not showing up?"
- Wait 1-2 minutes for GitHub Pages to rebuild
- Hard refresh your browser: `Cmd+Shift+R` (Mac) or `Ctrl+Shift+R` (Windows)

### "404 error on live site?"
- Make sure your main file is named `index.html`
- Check that Pages is enabled in Settings → Pages

### "Authentication error when pushing?"
- Use GitHub CLI: `gh auth login`
- Or use a personal access token

---

## Your Site URLs

Once deployed, you can access your site at:

- **GitHub Pages URL:** `https://username.github.io/repo-name/`
- **Direct GitHub link:** `https://github.com/username/repo-name`
- **Specific file:** `https://github.com/username/repo-name/blob/main/index.html`

---

**That's all you need to know!** 🎉

Deploy once, update anytime. No servers, no costs, completely free. 🚀
