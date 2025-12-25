# 🚀 NETLIFY DEPLOYMENT GUIDE - STEP BY STEP

## Complete Guide to Deploy Influencerium Frontend to Netlify

---

## 📋 STEP 1: Prepare Your GitHub Repository

### 1.1 Go to GitHub
- Visit: https://github.com/new
- Sign in with your GitHub account

### 1.2 Create New Repository
- **Repository name:** `influencerium-frontend`
- **Description:** "Influencerium - Creator-Brand Collaboration Platform"
- **Visibility:** Public (recommended for Netlify)
- **Initialize with:** Add a README file (optional - we have one)
- Click **"Create repository"**

### 1.3 Copy Repository URL
- After creation, you'll see a green "Code" button
- Copy the HTTPS URL (looks like: `https://github.com/yourusername/influencerium-frontend.git`)
- Save this URL - you'll need it in Step 2

---

## 📦 STEP 2: Push Files to GitHub

### 2.1 Open Terminal/Command Prompt
- **Windows:** Open Command Prompt or PowerShell
- **Mac/Linux:** Open Terminal

### 2.2 Navigate to Your Project Folder
```bash
# Create a folder for the project
mkdir influencerium-frontend
cd influencerium-frontend
```

### 2.3 Initialize Git Repository
```bash
git init
git add .
git commit -m "Initial commit: Influencerium frontend with 18 pages"
```

### 2.4 Add Remote Repository
Replace `YOUR_GITHUB_URL` with the URL you copied in Step 1.3:
```bash
git remote add origin YOUR_GITHUB_URL
git branch -M main
git push -u origin main
```

### 2.5 Verify on GitHub
- Go to your GitHub repository URL
- You should see all the HTML files uploaded ✅

---

## 🌐 STEP 3: Deploy to Netlify

### 3.1 Go to Netlify
- Visit: https://app.netlify.com
- Click **"Sign up"** or **"Log in"**
- Choose **"GitHub"** as your sign-up method
- Authorize Netlify to access your GitHub account

### 3.2 Create New Site
- Click **"New site from Git"** (or "Add new site")
- Select **"GitHub"** as your Git provider
- Search for **"influencerium-frontend"** repository
- Click to select it

### 3.3 Configure Build Settings
- **Branch to deploy:** `main`
- **Build command:** Leave empty (or use: `echo 'No build required'`)
- **Publish directory:** `.` (root directory)
- Click **"Deploy site"**

### 3.4 Wait for Deployment
- Netlify will automatically build and deploy
- You'll see a progress indicator
- Deployment usually takes 1-2 minutes

### 3.5 Get Your Live URL
- Once deployed, you'll see a URL like: `https://[random-name].netlify.app`
- This is your live website! 🎉

---

## 🎯 STEP 4: Customize Your Domain (Optional)

### 4.1 Change Site Name
- In Netlify dashboard, click **"Site settings"**
- Go to **"General"** → **"Site details"**
- Click **"Change site name"**
- Enter: `influencerium` (or your preferred name)
- Your URL becomes: `https://influencerium.netlify.app`

### 4.2 Add Custom Domain (Optional)
- In Netlify dashboard, go to **"Domain settings"**
- Click **"Add custom domain"**
- Enter your domain (e.g., `influencerium.com`)
- Follow DNS configuration instructions

---

## ✅ VERIFICATION CHECKLIST

After deployment, verify everything works:

- [ ] Landing page loads at root URL
- [ ] Navigation links work
- [ ] All 18 pages are accessible
- [ ] Responsive design works on mobile
- [ ] Images and styling load correctly
- [ ] No console errors in browser

---

## 🔗 USEFUL LINKS

- **Your GitHub Repository:** https://github.com/yourusername/influencerium-frontend
- **Your Netlify Site:** https://[sitename].netlify.app
- **Netlify Dashboard:** https://app.netlify.com
- **GitHub:** https://github.com

---

## 📧 NEXT STEPS

1. **Share your live URL** with stakeholders
2. **Gather feedback** on the design and UX
3. **Start Phase 1** - Backend Development (Dec 29)
4. **Integrate backend** with frontend (Week 6)

---

## 🆘 TROUBLESHOOTING

### Pages Not Loading
- Check that all HTML files are in the repository root
- Verify netlify.toml is configured correctly
- Clear browser cache and refresh

### Styling Not Showing
- Ensure CSS is inline in HTML files (not external)
- Check browser console for errors
- Verify file paths are correct

### Navigation Not Working
- Check that all HTML file names match the links
- Verify href attributes in navigation

### Need Help?
- Netlify Support: https://support.netlify.com
- GitHub Support: https://support.github.com

---

## 📊 DEPLOYMENT SUMMARY

| Step | Task | Time | Status |
|------|------|------|--------|
| 1 | Create GitHub Repository | 2 min | ⏳ |
| 2 | Push Files to GitHub | 5 min | ⏳ |
| 3 | Deploy to Netlify | 5 min | ⏳ |
| 4 | Customize Domain | 2 min | ⏳ |
| **Total** | **Complete Deployment** | **~15 min** | **⏳** |

---

**Good luck with your deployment! 🚀**

Once live, share your URL with James at hani_laid@yahoo.com
