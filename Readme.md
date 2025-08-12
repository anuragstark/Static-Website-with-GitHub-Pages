# GitHub Pages Deployment Guide

## Step-by-Step Instructions

### 1. Create Your Project Files

Create these files in a new folder on your computer:

**index.html** 

**styles.css** (optional - for external CSS):
```css
/* You can move the CSS from the <style> tags to this external file */
/* Then link it in your HTML with: <link rel="stylesheet" href="styles.css"> */
```

## Project Overview

# My GitHub Pages Website

A modern static website built with HTML, CSS, and JavaScript, deployed on GitHub Pages.

## Features
- Responsive design
- Modern CSS animations
- Glassmorphism effects
- Mobile-friendly

## Live Demo
[View Website](https://anuragstark.github.io/Static-Website-with-GitHub-Pages/)

## Local Development
Simply open `index.html` in your browser to view locally.

### 2. Create GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon → "New repository"
3. Name your repository (e.g., "my-static-website")
4. Make it **Public** (required for free GitHub Pages)
5. Check "Add a README file"
6. Click "Create repository"

### 3. Upload Your Files

**Method A: GitHub Web Interface**
1. In your new repo, click "Add file" → "Upload files"
2. Drag and drop your `index.html` file
3. Add a commit message: "Add initial website files"
4. Click "Commit changes"

**Method B: Command Line (if you have Git installed)**
```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
# Copy your index.html file here
git add .
git commit -m "Add initial website files"
git push origin main
```

### 4. Enable GitHub Pages

1. In your GitHub repository, click **Settings** (top menu)
2. Scroll down to **Pages** in the left sidebar
3. Under "Source", select **Deploy from a branch**
4. Choose **main** branch and **/ (root)** folder
5. Click **Save**

### 5. Access Your Live Website

1. GitHub will show you the URL (usually: `https://yourusername.github.io/repository-name`)
2. It may take 5-10 minutes to go live initially
3. Future updates go live in 1-2 minutes

### Domain Setup (Optional)
1. Buy a custom domain
2. In repo Settings → Pages → Custom domain
3. Add your domain and enable HTTPS

## Troubleshooting

**Site not loading?**
- Check that your main file is named `index.html`
- Ensure repository is public
- Wait 10 minutes for initial deployment

**CSS/JS not working?**
- Check file paths are correct
- Use relative paths (not absolute)
- Verify file names match exactly

**Updates not showing?**
- Hard refresh browser (Ctrl/Cmd + Shift + R)
- Check GitHub Actions tab for build status
- Wait a few minutes for deployment

## Example Repository Structure
```
your-repo-name/
├── index.html          # Main page (required)
├── about.html          # Additional pages
├── images/             # Images and assets
│   ├── logo.png
│   └── background.jpg
└── README.md           # Project documentation
```

## Notes

Your GitHub Pages site will automatically update whenever you push changes to your repository.