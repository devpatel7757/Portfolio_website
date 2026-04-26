# Devarshi Patel Portfolio — Setup & Deployment Guide

## 🚀 Option A: Open Instantly (Zero Setup)

Just double-click `index.html` in your file manager — it opens directly in any browser. No server needed.

---

## 🌐 Option B: Deploy to Vercel (Recommended — Free, Live URL)

### Step 1 — Install Git (if not installed)
Download from https://git-scm.com

### Step 2 — Create a GitHub repo
1. Go to https://github.com/new
2. Name it `portfolio` (or anything)
3. Leave it **public**
4. Click **Create repository**

### Step 3 — Push your file
```bash
# In your terminal, navigate to the folder with index.html
cd /path/to/your/portfolio-folder

git init
git add index.html
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/portfolio.git
git push -u origin main
```

### Step 4 — Deploy on Vercel
1. Go to https://vercel.com → Sign up with GitHub (free)
2. Click **"Add New Project"**
3. Select your `portfolio` repo
4. Click **Deploy** — Vercel auto-detects it as static HTML
5. Your site is live at: `https://portfolio-yourname.vercel.app`

**Custom domain (optional):** In Vercel → Project Settings → Domains → Add your domain (e.g., `devarshipatel.com`)

---

## 🌐 Option C: Deploy to GitHub Pages (Also Free)

1. Push `index.html` to GitHub (see Step 1-3 above)
2. Go to your repo → **Settings** → **Pages**
3. Under "Source", select **main branch**
4. Your site will be at: `https://yourusername.github.io/portfolio`

---

## ✏️ Customization Guide

### Add your real resume PDF for download
1. Save your resume as `resume.pdf` in the same folder as `index.html`
2. Find the "Download Resume" button in the HTML:
   ```html
   <a href="mailto:Devarshipatel535@gmail.com" class="btn-outline">
   ```
3. Change it to:
   ```html
   <a href="resume.pdf" download="Devarshi_Patel_Resume.pdf" class="btn-outline">
   ```

### Update LinkedIn / GitHub links
Search for `linkedin.com/in/devarshipatel7757` and `href="#"` (GitHub) and replace with your actual URLs.

### Update the GitHub link
Find the GitHub contact link section and replace `href="#"` with your actual GitHub URL.

### Add profile photo (optional)
In the About section, you can add:
```html
<img src="photo.jpg" alt="Devarshi Patel" style="width:100%;border-radius:16px;margin-bottom:1.5rem">
```
Place it before the `<div class="about-card-title">` line.

---

## 📁 File Structure
```
portfolio/
├── index.html        ← The entire website (single file)
├── resume.pdf        ← (Add your actual resume here)
└── DEPLOY.md         ← This guide
```

---

## 🎨 Features Included
- ✅ Dark / Light mode toggle
- ✅ Scroll progress indicator
- ✅ Animated hero particle network
- ✅ Animated stat counters (8.5M+, 497, 3.44 GPA)
- ✅ Skill progress bars with scroll-triggered animation
- ✅ Interactive project charts (Chart.js)
- ✅ Project filter buttons (All / Python / SQL / R)
- ✅ Timeline-style experience section
- ✅ Contact form with success animation
- ✅ Fully responsive (mobile + desktop)
- ✅ Glassmorphism + gradient design
- ✅ Smooth reveal animations on scroll
- ✅ Mobile hamburger menu
- ✅ SEO meta tags

---

## 🔧 Tech Stack
- Pure HTML5 / CSS3 / Vanilla JavaScript
- Chart.js (via CDN) for project visualizations
- Google Fonts: Syne + DM Sans
- No build tools, no npm, no dependencies to install
