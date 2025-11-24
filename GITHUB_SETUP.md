# GitHub Repository Setup Guide

## ✅ Repository Initialized

Your website is ready to be pushed to GitHub! Follow these steps:

## Step 1: Create GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the **"+"** icon in the top right → **"New repository"**
3. Fill in:
   - **Repository name**: `plant-phenotyping-website` (or your preferred name)
   - **Description**: "Website for A Data-Driven Image Analysis Pipeline for Plant Phenotyping in Greenhouse Environments"
   - **Visibility**: Choose **Public** (required for free GitHub Pages)
   - **DO NOT** initialize with README, .gitignore, or license (we already have these)
4. Click **"Create repository"**

## Step 2: Push Your Code

After creating the repository, GitHub will show you commands. Use these:

```bash
cd /home/grads/f/fahimehorvatinia/Documents/website

# Add the remote (replace YOUR_USERNAME and YOUR_REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# Or if you prefer SSH:
# git remote add origin git@github.com:YOUR_USERNAME/YOUR_REPO_NAME.git

# Commit your files (if not already committed)
git commit -m "Initial commit: Plant phenotyping website"

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** (top menu)
3. Scroll down to **"Pages"** in the left sidebar
4. Under **"Source"**:
   - Select **"Deploy from a branch"**
   - Branch: **`main`**
   - Folder: **`/ (root)`**
5. Click **"Save"**
6. Your website will be live at:
   - `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`

## Step 4: Wait for Deployment

- GitHub Pages usually takes 1-2 minutes to deploy
- You'll see a green checkmark when it's ready
- The URL will be shown in the Pages settings

## Optional: Custom Domain

If you want a custom domain (e.g., `yourname.tamu.edu`):
1. Create a file named `CNAME` in the root directory
2. Add your domain name (one line): `yourname.tamu.edu`
3. Commit and push
4. Configure DNS with your domain provider

## Files Included

✅ `index.html` - Main website file
✅ `css/` - Stylesheets
✅ `js/` - JavaScript files
✅ `images/` - All images
✅ `README.md` - Project documentation
✅ `.gitignore` - Git ignore rules

## Files Excluded (by .gitignore)

- `PRMI-main-extracted/` - Extracted files
- `*.zip` - Zip archives
- `*.tmp`, `*.log` - Temporary files

## Need Help?

- GitHub Pages docs: https://pages.github.com
- Git basics: https://git-scm.com/doc

