---
layout: post
title: "Deploying to GitHub Pages"
date: 2026-03-01 09:00:00 +0000
categories: deployment github
---

GitHub Pages is a great way to host static websites directly from your GitHub repository. In this post, I'll walk you through the process of deploying your Jekyll site to GitHub Pages.

## Prerequisites

- A GitHub account
- A GitHub repository with a GitHub Pages-compatible name (e.g., `username.github.io`)
- Jekyll installed locally
- Git installed

## Step 1: Set Up Your Repository

If you're using the repository naming convention `username.github.io`, any content pushed to the `main` or `master` branch will automatically be published.

## Step 2: Update Your Site

Make sure your Jekyll site is configured properly:

1. Update `_config.yml` with your site information
2. Build your site locally: `bundle exec jekyll build`
3. Test your site: `bundle exec jekyll serve`

## Step 3: Push to GitHub

Once you're happy with your site:

```bash
git add .
git commit -m "Initial Jekyll site"
git push origin main
```

## Step 4: Enable GitHub Pages

1. Go to your repository settings
2. Navigate to the "Pages" section
3. Select the branch to deploy from (usually `main` or `master`)
4. Save your settings

## Step 5: View Your Site

After a few minutes, your site will be live at `https://username.github.io`.

## Tips

- Keep your repository public for free hosting
- Consider adding a custom domain in your repository settings
- Use GitHub Actions for automated builds and deployments
- Always test locally before pushing to production

That's it! Your Jekyll site is now live on GitHub Pages. Happy blogging!
