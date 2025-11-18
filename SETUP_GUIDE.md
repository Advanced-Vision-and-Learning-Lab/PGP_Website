# Website Setup Guide

## ✅ What's Already Done

Your website structure is complete with:
- ✅ Main HTML file (`index.html`)
- ✅ CSS framework files
- ✅ JavaScript files
- ✅ Hero section with greenhouse background
- ✅ All sections and content from your paper
- ✅ Links to Hugging Face demo and documentation

## 📋 Step-by-Step Checklist

### 1. Add Missing Images (Optional but Recommended)

Add these images to the `images/` folder for a complete website:

#### Dataset Sample Images (for the Dataset Samples section):
- `sample_corn.png` - One representative corn image
- `sample_cotton.png` - One representative cotton image  
- `sample_rice.png` - One representative rice image
- `sample_sorghum.png` - One representative sorghum image

**Note:** The website will show placeholder text if these images are missing, so it's functional without them.

#### Material Icons (Optional):
- `arxiv.jpg` - ArXiv logo (for paper link)
- `dataset.png` - Dataset icon
- `code.png` - Code/GitHub icon
- `docs.png` - Documentation icon

**Note:** The website has fallback placeholders for these, so they're optional.

### 2. Update Paper Link

Edit `index.html` and find the line with:
```html
<a href="">Paper</a>
```

Replace the empty `href=""` with your actual paper URL (arXiv, journal, etc.)

### 3. Update Citation Information

In the Citation section, update:
- Conference/Journal name
- Year of publication
- Any other publication details

### 4. Test Locally

1. **Open in browser:**
   ```bash
   cd /home/grads/f/fahimehorvatinia/Documents/website
   # Then open index.html in your browser
   ```

2. **Or use a local server (recommended):**
   ```bash
   # Python 3
   python3 -m http.server 8000
   
   # Then open: http://localhost:8000
   ```

3. **Check:**
   - All images load correctly
   - All links work
   - Layout looks good on desktop and mobile
   - Text is readable

### 5. Deploy to GitHub Pages (Recommended)

#### Option A: Create a New Repository

1. **Create a new GitHub repository:**
   - Go to GitHub.com
   - Click "New repository"
   - Name it (e.g., `plant-phenotyping-website`)
   - Make it public (required for free GitHub Pages)
   - Don't initialize with README

2. **Upload your files:**
   ```bash
   cd /home/grads/f/fahimehorvatinia/Documents/website
   
   # Initialize git (if not already)
   git init
   
   # Add all files
   git add .
   
   # Commit
   git commit -m "Initial website commit"
   
   # Add your GitHub repository as remote
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   
   # Push to GitHub
   git branch -M main
   git push -u origin main
   ```

3. **Enable GitHub Pages:**
   - Go to your repository on GitHub
   - Click "Settings" → "Pages"
   - Under "Source", select "Deploy from a branch"
   - Select branch: `main` and folder: `/ (root)`
   - Click "Save"
   - Your site will be available at: `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`

#### Option B: Use Existing Repository

If you already have a repository, just push the website files to it and enable GitHub Pages in the same way.

### 6. Alternative Deployment Options

#### Netlify (Easy drag-and-drop):
1. Go to [netlify.com](https://netlify.com)
2. Sign up/login
3. Drag and drop your `website` folder
4. Get instant URL

#### Your Institution's Web Server:
- Contact your IT department
- Upload files via FTP/SFTP
- They'll provide the URL

### 7. Custom Domain (Optional)

If you want a custom domain (e.g., `yourname.tamu.edu`):
- GitHub Pages: Add CNAME file with your domain
- Netlify: Configure in domain settings
- Contact your institution's IT for subdomain setup

## 📁 Final File Structure

Your website should have this structure:
```
website/
├── index.html
├── css/
│   ├── normalize.css
│   ├── skeleton.css
│   └── footable.*.css
├── js/
│   ├── jquery.min.js
│   └── footable.*.js
├── images/
│   ├── Automated-precision-phenotyping-greenhouse.jpg ✅
│   ├── flow.jpg ✅
│   ├── logo.png ✅
│   ├── workflow.png ✅
│   ├── sample_corn.png (optional)
│   ├── sample_cotton.png (optional)
│   ├── sample_rice.png (optional)
│   ├── sample_sorghum.png (optional)
│   └── [other optional icons]
├── README.md
└── SETUP_GUIDE.md (this file)
```

## 🎨 Customization Tips

1. **Colors:** Edit the CSS in `<style>` section of `index.html` to match your preferences
2. **Content:** Update any text in `index.html` as needed
3. **Images:** Replace any images in `images/` folder
4. **Links:** Update all `href` attributes with your actual URLs

## ✅ Quick Start (Minimal Setup)

If you want to deploy immediately with minimal setup:

1. **Update paper link** in `index.html`
2. **Test locally** by opening `index.html` in browser
3. **Deploy to GitHub Pages:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin YOUR_REPO_URL
   git push -u origin main
   ```
4. **Enable GitHub Pages** in repository settings

That's it! Your website will be live.

## 🆘 Troubleshooting

- **Images not showing?** Check file paths are correct (case-sensitive on Linux)
- **CSS not loading?** Ensure `css/` folder is in the same directory as `index.html`
- **GitHub Pages not working?** Make sure repository is public and branch is `main` or `master`

## 📞 Need Help?

- GitHub Pages docs: https://pages.github.com
- Check your browser console (F12) for any errors
- Verify all file paths are relative (start with `./`)

