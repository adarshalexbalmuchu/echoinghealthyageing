# 🚀 GitHub Pages Deployment Guide

Follow these steps to deploy your "Echoing Healthy Ageing" project to GitHub Pages.

## Step 1: Initialize Git Repository

Open PowerShell in your project directory and run:

```powershell
cd "c:\Users\adars\Downloads\adarshalexbalmuchu.github.io\echoinghealthyageing"
git init
git add .
git commit -m "Initial commit - Echoing Healthy Ageing interactive strategy"
```

## Step 2: Create GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon → "New repository"
3. Repository name: `echoinghealthyageing` (or any name you prefer)
4. Set it to **Public** (required for free GitHub Pages)
5. **Don't** initialize with README (we already have one)
6. Click "Create repository"

## Step 3: Connect Local Repository to GitHub

Copy the commands from GitHub's "push an existing repository" section, which will look like:

```powershell
git remote add origin https://github.com/YOUR_USERNAME/echoinghealthyageing.git
git branch -M main
git push -u origin main
```

Replace `YOUR_USERNAME` with your actual GitHub username.

## Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" in the sidebar
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"

## Step 5: Access Your Live Site

After 2-5 minutes, your site will be available at:
`https://YOUR_USERNAME.github.io/echoinghealthyageing/`

GitHub will show you the exact URL in the Pages settings.

## Step 6: Configure AI Features (Optional)

To enable the full AI-powered insights:

### Get a Gemini API Key:
1. Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Sign in with your Google account
3. Click "Create API Key"
4. Copy the generated key

### Add the API Key:
1. Open `index.html` in any text editor
2. Find this line (around line 335):
   ```javascript
   const GEMINI_API_KEY = ''; // Add your Gemini API key here for AI features
   ```
3. Replace it with:
   ```javascript
   const GEMINI_API_KEY = 'YOUR_ACTUAL_API_KEY_HERE';
   ```
4. Save the file

### Deploy the Update:
```powershell
git add index.html
git commit -m "Add Gemini API key for AI features"
git push
```

## 🎉 You're Done!

Your site is now live! The application will work perfectly without the API key (showing helpful fallback content), but with the API key, users will get personalized AI-generated insights.

## Updating Your Site

To make changes in the future:

```powershell
# Make your changes, then:
git add .
git commit -m "Describe your changes"
git push
```

Changes will appear on your live site within a few minutes.

## Troubleshooting

- **Site not loading?** Check the Pages settings and ensure the source is set correctly
- **404 errors?** Make sure your main file is named `index.html`
- **API not working?** Verify your API key is correct and has no extra spaces
- **Changes not appearing?** GitHub Pages can take 2-5 minutes to update

## Security Note

**Important**: Never commit API keys to public repositories in production. For this demo project, it's acceptable, but consider using environment variables or server-side solutions for production applications.
