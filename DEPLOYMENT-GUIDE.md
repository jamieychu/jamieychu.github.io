# GitHub Pages Deployment Guide

## 🚀 DEPLOYMENT STEPS

### Step 1: Create GitHub Repository

1. Go to [github.com](https://github.com) and click **New Repository**
2. Repository name: `jamieychu.github.io` (MUST match your username)
3. Description: "Jamie Chu - Product Manager Portfolio"
4. Set to **Public**
5. Do NOT initialize with README (we have our own)
6. Click **Create Repository**

### Step 2: Upload Files to GitHub

**Option A - Via GitHub Web Interface (Easiest):**
1. Click **uploading an existing file**
2. Drag all files from portfolio-repo folder:
   - index.html
   - chibiotaku-v1.glb
   - README.md
   - CNAME
   - .gitignore
3. Commit message: "Initial portfolio deployment"
4. Click **Commit changes**

**Option B - Via Git Command Line:**
```bash
cd portfolio-repo
git init
git add .
git commit -m "Initial portfolio deployment"
git branch -M main
git remote add origin https://github.com/jamieychu/jamieychu.github.io.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to repository Settings → Pages (left sidebar)
2. Source: **Deploy from a branch**
3. Branch: **main** 
4. Folder: **/ (root)**
5. Click **Save**

⏳ Wait 2-3 minutes for initial deployment

**Test:** Visit `https://jamieychu.github.io` - your portfolio should be live!

### Step 4: Configure Custom Domain (jamchu.cool)

**A. In GitHub:**
1. Go to Settings → Pages
2. Custom domain: Enter `jamchu.cool`
3. Click **Save**
4. Check **Enforce HTTPS** (wait a few minutes for certificate)

**B. In GoDaddy DNS Settings:**
1. Log in to GoDaddy → My Products → DNS
2. **Delete** any existing A records for `@`
3. **Add these 4 A records** (Type: A, Name: @, TTL: 1 hour):
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
4. **Add CNAME record** (Type: CNAME, Name: www, Value: `jamieychu.github.io`, TTL: 1 hour)

⏳ DNS propagation: 10 minutes - 24 hours (usually ~1 hour)

**Verify:** Visit `jamchu.cool` - should redirect to your portfolio

---

## ✅ FINAL VERIFICATION CHECKLIST

- [ ] `jamchu.cool` shows portfolio
- [ ] `www.jamchu.cool` redirects to jamchu.cool
- [ ] All navigation links work
- [ ] Project 1 iframe loads Pokemon Blue Gacha demo
- [ ] "View Demo" opens `jamieychu.github.io/pokemon_blue_gacha`
- [ ] 3D chibi model loads and spins
- [ ] Inspiration mosaic expands/collapses
- [ ] Mobile responsive (test on phone)
- [ ] HTTPS enabled (green lock icon)

---

## 🎮 FUTURE PROJECTS

When you add more projects (Crunchyroll Otaku, Webtoon QoL):

1. Create separate GitHub repos for each project
2. Enable GitHub Pages on each repo
3. Update portfolio `index.html` to link to new project URLs
4. Your projects will be at:
   - `jamieychu.github.io/pokemon-blue-gacha`
   - `jamieychu.github.io/crunchyroll-otaku`
   - `jamieychu.github.io/webtoon-qol`

**No subdomain setup needed!** GitHub Pages URLs are professional for portfolio projects.

---

## 🐛 TROUBLESHOOTING

**Portfolio not loading:**
- Check GitHub Pages is enabled (Settings → Pages)
- Verify CNAME file contains `jamchu.cool`
- Check DNS propagation: https://dnschecker.org

**Project iframe not loading:**
- Verify Pokemon Blue Gacha repo has GitHub Pages enabled
- Check iframe URL in browser directly
- Look for console errors (F12 → Console)

**3D chibi not appearing:**
- Verify `chibiotaku-v1.glb` is in root directory with `index.html`
- Check browser console for errors (F12)

**Certificate/HTTPS issues:**
- Uncheck then re-check "Enforce HTTPS" in GitHub Pages
- Wait 10-15 minutes for certificate generation
- Clear browser cache

---

## 📝 MAINTENANCE NOTES

**To update portfolio:**
1. Edit `index.html` locally
2. Upload to GitHub (replace file or git push)
3. Changes appear in 1-2 minutes

**To update currently ticker:**
- Edit lines ~3178-3207 in index.html
- Update emoji, text, and values as desired

**To add new projects:**
- Duplicate project block in index.html
- Update content, links, and preview images
- Add navigation circle in project-nav section

---

## 🎉 YOU'RE DONE!

Your portfolio is now live with a professional custom domain!

**Main site:** jamchu.cool  
**Projects:** jamieychu.github.io/[project-name]

Simple, clean, and professional. Time to celebrate! 🚀✨
