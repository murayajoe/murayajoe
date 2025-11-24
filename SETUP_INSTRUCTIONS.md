# 🚀 GitHub Profile Setup Instructions

This guide will walk you through setting up your professional GitHub profile with auto-updating features.

---

## 📋 Prerequisites

- A GitHub account (username: **murayajoe**)
- Git installed on your local machine
- Basic knowledge of Git commands
- A YouTube channel (for video integration)

---

## 🏗️ Step 1: Create the GitHub Repository

### **CRITICAL: The repository MUST be named exactly as your username**

1. Go to [GitHub](https://github.com/new)
2. Repository name: **murayajoe** (must match your username exactly)
3. Description: "My professional GitHub profile"
4. Set to **Public** (required for profile README to work)
5. Do **NOT** initialize with README, .gitignore, or license
6. Click "Create repository"

> ⚠️ **Important**: GitHub automatically displays the README.md from a repository named after your username on your profile page.

---

## ⚙️ Step 2: Enable GitHub Actions

1. Go to your repository settings
2. Navigate to **Settings** → **Actions** → **General**
3. Under "Workflow permissions", select:
   - ✅ **Read and write permissions**
   - ✅ **Allow GitHub Actions to create and approve pull requests**
4. Click **Save**

Without these permissions, your automated workflows won't be able to update the README.

---

## 🎥 Step 3: Get Your YouTube Channel ID

Your YouTube channel ID is needed to automatically pull in your latest videos.

### Method 1: From YouTube Studio
1. Go to [YouTube Studio](https://studio.youtube.com)
2. Click on **Settings** → **Channel** → **Advanced settings**
3. Copy your **Channel ID**

### Method 2: From Your Channel Page (Recommended)
1. Go to your YouTube channel (@kenyansenpai)
2. Right-click anywhere on the page and select "View Page Source"
3. Press `Ctrl+F` (or `Cmd+F` on Mac) and search for: `"channelId"`
4. Copy the ID that looks like: `UCxxxxxxxxxxxxxxxxxxxxx`

### Update the Workflow File
1. Open `.github/workflows/blog-post-workflow.yml`
2. Find the line: `feed_list: "https://www.youtube.com/feeds/videos.xml?channel_id=YOUR_CHANNEL_ID_HERE"`
3. Replace `YOUR_CHANNEL_ID_HERE` with your actual channel ID
4. Save the file

---

## 📝 Step 4: Replace Placeholders

### In `README.md`:
- ✅ All username references already use "murayajoe"
- ✅ All social media links are already configured
- ✅ Email is already set to joemuraya90@gmail.com

### If you have a blog on dev.to or Medium:
1. Open `.github/workflows/blog-post-workflow.yml`
2. Find: `feed_list: "https://dev.to/feed/YOUR_USERNAME_HERE"`
3. Replace with your actual username, or remove this job if you don't have a blog

### Project Repositories:
The README references two placeholder repositories:
- `odoo-custom-modules`
- `kenya-erp-solutions`

**Options:**
- Create these repositories to showcase your projects
- Or edit the README to reference your actual repository names

---

## 🚢 Step 5: Deploy to GitHub

### Initialize Git Repository
```bash
cd "c:\Users\joemu\OneDrive - Anqad Systems Ltd\Desktop\gut muraya"
git init
git add .
git commit -m "🎉 Initial commit: Professional GitHub profile setup"
```

### Connect to GitHub
```bash
git branch -M main
git remote add origin https://github.com/murayajoe/murayajoe.git
git push -u origin main
```

### If you get authentication errors:
You need to use a Personal Access Token (PAT):

1. Go to [GitHub Settings → Developer settings → Personal access tokens → Tokens (classic)](https://github.com/settings/tokens)
2. Click "Generate new token (classic)"
3. Give it a name like "Profile Repository"
4. Select scopes:
   - ✅ `repo` (all repository permissions)
   - ✅ `workflow` (update GitHub Action workflows)
5. Click "Generate token" and **COPY IT IMMEDIATELY**
6. When pushing, use:
   ```bash
   git push https://YOUR_TOKEN@github.com/murayajoe/murayajoe.git main
   ```

---

## ▶️ Step 6: Manually Trigger Workflows

After pushing to GitHub:

1. Go to your repository on GitHub
2. Click on the **Actions** tab
3. You should see three workflows:
   - 📺 Latest YouTube Videos and Blog Posts
   - 🐍 Generate Snake Animation
   - 📊 Update Stats

### Run Each Workflow Manually (First Time):
1. Click on each workflow name
2. Click the **"Run workflow"** dropdown on the right
3. Click **"Run workflow"** button
4. Wait for it to complete (green checkmark)

### Expected Results:
- **Snake Animation**: Creates an `output` branch with snake SVG/GIF files
- **YouTube Videos**: Updates README with your latest 6 videos (if channel ID is configured)
- **Update Stats**: Creates a timestamp file

> 💡 **Note**: The stats cards (GitHub stats, streak, etc.) update automatically without workflows - they're generated on-demand by external services.

---

## 🔧 Troubleshooting Common Issues

### Issue 1: "Resource not accessible by integration"
**Solution**: Enable write permissions in Settings → Actions → General → Workflow permissions

### Issue 2: Snake animation not showing
**Solution**:
- Ensure the workflow ran successfully
- Check that an `output` branch was created
- Wait 5-10 minutes for GitHub's CDN to update
- Clear your browser cache

### Issue 3: YouTube videos not updating
**Solution**:
- Verify your Channel ID is correct
- Ensure the channel has public videos
- Check that the workflow ran without errors
- The RSS feed must be public (not private channel)

### Issue 4: Stats cards showing "404" or not loading
**Solution**:
- This is normal for brand new accounts
- Wait 24 hours for GitHub's API to index your profile
- Make a few commits to generate activity
- The services need public activity to display

### Issue 5: Workflow fails with "push declined"
**Solution**:
- Check that Actions have write permissions
- Verify your email in commit settings matches GitHub email
- Try re-running the workflow

---

## 🎨 Step 7: Customize Your Profile

See [CUSTOMIZATION_GUIDE.md](CUSTOMIZATION_GUIDE.md) for detailed customization options including:
- Changing color schemes
- Adding/removing sections
- Modifying stat card themes
- Adding new badges and integrations

---

## 📊 Verification Checklist

After setup, verify everything works:

- [ ] Repository named "murayajoe" exists and is public
- [ ] README.md is visible on your GitHub profile page
- [ ] All social media badges link to correct profiles
- [ ] GitHub Actions have write permissions enabled
- [ ] All three workflows exist in Actions tab
- [ ] Snake animation workflow completed successfully
- [ ] YouTube channel ID is configured (if desired)
- [ ] Stats cards are loading (may take 24 hours for new accounts)
- [ ] Contribution graph is visible
- [ ] Typing animation works on profile

---

## 🔄 Maintenance

### Auto-Updates:
- **Hourly**: YouTube videos refresh
- **Every 6 hours**: Snake animation regenerates
- **Daily**: Stats cache refreshes

### Manual Updates:
- Social links: Edit README.md directly
- Tech stack: Add/remove badges in README.md
- Goals: Update the JavaScript goals section
- Projects: Update featured repository links

---

## 📚 Additional Resources

- [GitHub Profile README Guide](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)
- [GitHub Actions Documentation](https://docs.github.com/en/actions)
- [Shields.io Badge Generator](https://shields.io/)
- [GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats)
- [Capsule Render](https://github.com/kyechan99/capsule-render)
- [Blog Post Workflow](https://github.com/gautamkrishnar/blog-post-workflow)

---

## 🆘 Need Help?

If you encounter issues:
1. Check the [Troubleshooting](#-troubleshooting-common-issues) section above
2. Review workflow logs in the Actions tab
3. Verify all placeholders are replaced
4. Ensure all files are in correct directories
5. Check that repository is public and named correctly

---

## 🎉 Success!

Once everything is set up, your profile will:
- ✨ Auto-update with latest YouTube videos
- 📊 Display real-time GitHub statistics
- 🐍 Show animated contribution snake
- 🎯 Showcase your tech stack and projects
- 🤝 Provide easy connection to all your socials

**Your professional GitHub presence is now live!** 🚀

Visit your profile at: https://github.com/murayajoe
