# Satwa Media Website

## 🚀 Deploy to Vercel (Free) + Connect GoDaddy Domain

---

### STEP 1 — Upload to GitHub (free)

1. Go to https://github.com and create a free account (if you don't have one)
2. Click **"New repository"** → name it `satwa-media` → click **Create**
3. On your computer, install Git: https://git-scm.com/downloads
4. Open Terminal / Command Prompt and run:

```bash
cd satwa-media
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/satwa-media.git
git push -u origin main
```

---

### STEP 2 — Deploy on Vercel (free)

1. Go to https://vercel.com and sign up with your GitHub account
2. Click **"Add New Project"**
3. Select your `satwa-media` repository
4. Leave all settings as default — click **Deploy**
5. ✅ Your site is now live at `satwa-media.vercel.app`

---

### STEP 3 — Connect Your GoDaddy Domain

**In Vercel:**
1. Go to your project → **Settings** → **Domains**
2. Type your domain (e.g. `satwamedia.in`) → click **Add**
3. Vercel will show you DNS records to add — note them down

**In GoDaddy:**
1. Log in to https://godaddy.com
2. Go to **My Products** → find your domain → click **DNS**
3. Delete the existing **A record** (if any)
4. Click **Add** → choose type **A**:
   - Name: `@`
   - Value: `76.76.21.21` (Vercel's IP)
   - TTL: 600
5. Click **Add** again → choose type **CNAME**:
   - Name: `www`
   - Value: `cname.vercel-dns.com`
   - TTL: 600
6. Save changes

⏱️ Wait 10–30 minutes for DNS to propagate.

**Back in Vercel:**
- Your domain status will change to ✅ **Valid**

---

### ✅ Done! Your website is live on your domain.

For support: satwamediaa@gmail.com
