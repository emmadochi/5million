# 🚀 GitHub Deployment Guide

## Step 1: Create GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the **"+"** icon in the top right corner
3. Select **"New repository"**
4. Repository name: `5million` (or any name you prefer)
5. Description: "Professional website and app developer landing page"
6. Choose **Public** (for free GitHub Pages) or **Private**
7. **DO NOT** initialize with README, .gitignore, or license (we already have these)
8. Click **"Create repository"**

## Step 2: Connect Local Repository to GitHub

After creating the repository, GitHub will show you commands. Use these:

### Option A: If you haven't pushed yet (Recommended)

```bash
git remote add origin https://github.com/YOUR_USERNAME/5million.git
git branch -M main
git push -u origin main
```

Replace `YOUR_USERNAME` with your actual GitHub username.

### Option B: If repository already exists on GitHub

```bash
git remote add origin https://github.com/YOUR_USERNAME/5million.git
git branch -M main
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Scroll down to **Pages** (left sidebar)
4. Under **Source**, select:
   - Branch: `main` (or `master`)
   - Folder: `/ (root)`
5. Click **Save**
6. Your site will be live at: `https://YOUR_USERNAME.github.io/5million/`

## Step 4: Verify Deployment

- Wait 1-2 minutes for GitHub Pages to build
- Visit your site URL
- Check all pages work correctly
- Test on mobile devices

## 🔄 Updating Your Site

Whenever you make changes:

```bash
git add .
git commit -m "Description of your changes"
git push
```

GitHub Pages will automatically update within 1-2 minutes.

## 📝 Custom Domain (Optional)

If you have a custom domain:

1. Go to repository **Settings > Pages**
2. Enter your domain in **Custom domain**
3. Add a `CNAME` file to your repository root:
   ```
   yourdomain.com
   ```
4. Update your DNS settings (add CNAME record pointing to `YOUR_USERNAME.github.io`)

## 🛠️ Troubleshooting

### If push is rejected:
```bash
git pull origin main --allow-unrelated-histories
git push -u origin main
```

### If GitHub Pages shows 404:
- Check that `index.html` is in the root directory
- Verify branch is set to `main` or `master` in Pages settings
- Wait a few minutes for deployment to complete

### If styles/images don't load:
- Ensure all file paths are relative (not absolute)
- Check file names match exactly (case-sensitive on Linux servers)

## ✅ Checklist

- [ ] GitHub repository created
- [ ] Local repository connected to GitHub
- [ ] Code pushed to GitHub
- [ ] GitHub Pages enabled
- [ ] Site is live and accessible
- [ ] All pages load correctly
- [ ] Mobile responsive design works
- [ ] WhatsApp links work
- [ ] Portfolio pages accessible

## 🎉 You're Done!

Your professional landing page is now live on GitHub Pages!

**Live URL**: `https://YOUR_USERNAME.github.io/5million/`

Share this URL with clients and prospects!

