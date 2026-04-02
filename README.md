# AUREA — NASA Mars Food Challenge

**Autonomous Unified Regenerative Ecosystem for Agriculture**  
Submitted by Shiann Davis · SD Davis Enterprises · 2025

---

## Deploy in 5 Steps

### 1. Create GitHub Repo
```bash
# On github.com → New Repository
# Name: aurea-proposal
# Visibility: Public (required for free GitHub Pages)
# Don't add README (you already have files)
```

### 2. Push Files
```bash
cd aurea-site
git init
git add .
git commit -m "🚀 Initial AUREA deployment"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/aurea-proposal.git
git push -u origin main
```

### 3. Enable GitHub Pages
1. Go to repo → **Settings** → **Pages**
2. Source: **GitHub Actions**
3. The workflow auto-runs on every push

### 4. Set Custom Domain

**Option A — Subdomain (recommended):**
Use `aurea.sddavisenterprises.com` or similar

In your DNS provider (Cloudflare recommended):
```
Type:  CNAME
Name:  aurea
Value: YOUR_USERNAME.github.io
TTL:   Auto
```

**Option B — Root domain:**
Use `aurea-mars.com` or any domain you own

In your DNS:
```
Type:  A
Name:  @
Value: 185.199.108.153
       185.199.109.153
       185.199.110.153
       185.199.111.153
```

Then update `CNAME` file to match your domain exactly.

### 5. Enforce HTTPS
- Go to repo → **Settings** → **Pages**
- Check **Enforce HTTPS** (appears after DNS propagates, ~5 min on Cloudflare)

---

## Update the Domain

Edit the `CNAME` file — one line, your domain only:
```
aurea.yourdomain.com
```

---

## Update Content

Edit `index.html` and push:
```bash
git add index.html
git commit -m "Update proposal content"
git push
```

GitHub Actions auto-deploys within ~60 seconds.

---

## File Structure
```
aurea-proposal/
├── index.html              ← Full proposal site
├── CNAME                   ← Custom domain
├── README.md               ← This file
└── .github/
    └── workflows/
        └── deploy.yml      ← Auto-deploy CI/CD
```

---

*AUREA · SD Davis Enterprises · Ozark, MO*
