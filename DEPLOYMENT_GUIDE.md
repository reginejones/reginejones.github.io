# Quick Deployment Guide for Regine Jones Portfolio

Follow these simple steps to get your portfolio live on GitHub Pages!

## Prerequisites
- A GitHub account (sign up at github.com if you don't have one)
- Git installed on your computer (download from git-scm.com)

## Step-by-Step Instructions

### 1️⃣ Create Your GitHub Repository

1. Go to https://github.com and sign in
2. Click the **+** button (top right) → **New repository**
3. Repository settings:
   - **Name**: `YOUR_USERNAME.github.io` (replace YOUR_USERNAME with your actual GitHub username)
   - **Visibility**: Public
   - **DON'T** check "Initialize this repository with a README"
4. Click **Create repository**

### 2️⃣ Open Terminal in Project Folder

**On Mac:**
- Open Terminal
- Navigate to your project: `cd path/to/your/project`

**On Windows:**
- Open Command Prompt or Git Bash
- Navigate to your project: `cd path\to\your\project`

### 3️⃣ Run These Commands

Copy and paste these commands one at a time:

```bash
# Initialize git
git init

# Add all files
git add .

# Make your first commit
git commit -m "Initial commit: Regine Jones portfolio"

# Set the default branch to main
git branch -M main

# Connect to your GitHub repository
# ⚠️ IMPORTANT: Replace YOUR_USERNAME with your actual GitHub username!
git remote add origin https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io.git

# Push to GitHub
git push -u origin main
```

**Note:** When you run the push command, you may be asked to sign in to GitHub. Follow the prompts!

### 4️⃣ Enable GitHub Pages

1. Go to your repository on GitHub: `https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io`
2. Click **Settings** (top menu bar)
3. Scroll down and click **Pages** in the left sidebar
4. Under **Source**:
   - Branch: Select **main**
   - Folder: Select **/ (root)**
5. Click **Save**

### 5️⃣ Wait and View! 🎉

- Your site will be live at: `https://YOUR_USERNAME.github.io`
- It takes 1-5 minutes to deploy
- Refresh the GitHub Pages settings page to see the green success message

## 🔄 How to Update Your Site

After making changes to your files:

```bash
git add .
git commit -m "Updated portfolio"
git push
```

Your changes will be live in a few minutes!

## 🆘 Common Issues

### "fatal: not a git repository"
- Make sure you're in the correct folder
- Run `git init` first

### "Permission denied"
- You may need to set up SSH keys or use HTTPS authentication
- GitHub will prompt you to sign in

### "Site not loading"
- Wait a few minutes - deployment takes time
- Check that repository name is EXACTLY `YOUR_USERNAME.github.io`
- Verify GitHub Pages is enabled in Settings

### "Images not showing"
- Make sure images are in the `assets/` folder
- Check image file names match what's in the HTML
- Use relative paths: `assets/image.jpg`

## ✅ Checklist Before Going Live

- [ ] Updated name and personal info in `index.html`
- [ ] Added your photo to `assets/` folder
- [ ] Updated social media links
- [ ] Added your projects with descriptions
- [ ] Updated work experience
- [ ] Changed email address in contact section
- [ ] Tested on mobile and desktop locally
- [ ] Committed and pushed to GitHub
- [ ] Enabled GitHub Pages
- [ ] Verified site is live

## 🎯 Next Steps

1. Share your portfolio URL with recruiters!
2. Add it to your resume and LinkedIn
3. Keep it updated with new projects
4. Consider adding Google Analytics to track visitors

## 💡 Pro Tips

- Use a consistent color scheme that represents your brand
- Keep project descriptions concise but impactful
- Update regularly with new projects and skills
- Get feedback from peers before sharing widely
- Make sure all links work before going live

---

**You've got this! 🚀**

If you run into any issues, check the main README.md for more detailed troubleshooting.
