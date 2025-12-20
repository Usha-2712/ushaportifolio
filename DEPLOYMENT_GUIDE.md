# How to Deploy Your Portfolio to GitHub Pages

## Step 1: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Name it (e.g., `ushaportifolio` or `portfolio`)
5. Make it **Public** (required for free GitHub Pages)
6. Don't initialize with README, .gitignore, or license
7. Click "Create repository"

## Step 2: Initialize Git in Your Project Folder

Open your terminal/command prompt in your project folder and run:

```bash
# Initialize git repository
git init

# Add all files
git add .

# Create your first commit
git commit -m "Initial commit: Portfolio website"

# Add your GitHub repository as remote (replace YOUR_USERNAME and REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Replace:**
- `YOUR_USERNAME` with your GitHub username (e.g., `Usha-2712`)
- `REPO_NAME` with your repository name (e.g., `ushaportifolio`)

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings** tab
3. Scroll down to **Pages** in the left sidebar
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**

## Step 4: Rename Your File

You need to rename `portfolio.html` to `index.html` so GitHub Pages can find it:

**Option A: Using File Explorer (Windows)**
- Rename `portfolio.html` to `index.html` in your file explorer

**Option B: Using Git commands**
```bash
git mv portfolio.html index.html
git commit -m "Rename portfolio.html to index.html"
git push
```

## Step 5: Access Your Website

After a few minutes, your portfolio will be live at:

**Format:** `https://YOUR_USERNAME.github.io/REPO_NAME/`

**Example:** 
- If your username is `Usha-2712` and repo is `ushaportifolio`:
- URL: `https://usha-2712.github.io/ushaportifolio/`

If you name your repository exactly `YOUR_USERNAME.github.io`, then:
- URL: `https://YOUR_USERNAME.github.io/` (shorter URL!)

## Troubleshooting

### If the site doesn't load:
- Wait 5-10 minutes after enabling Pages
- Check Settings → Pages to see the status
- Make sure `index.html` is in the root of your repository
- Clear your browser cache

### To update your site:
```bash
# After making changes to your files
git add .
git commit -m "Update portfolio"
git push
```
Changes will appear on your live site in a few minutes.

## Quick Checklist

- [ ] Created GitHub repository
- [ ] Initialized git in project folder
- [ ] Added and committed files
- [ ] Pushed to GitHub
- [ ] Renamed `portfolio.html` to `index.html`
- [ ] Enabled GitHub Pages in repository settings
- [ ] Waited a few minutes for deployment
- [ ] Tested the live URL

Your portfolio is now live! 🎉


