# Axiogrid Website Deployment

## Quick Deploy to Vercel (Easiest Method)

### Option A: Deploy via Vercel CLI (Recommended)

1. Install Vercel CLI:
   ```bash
   npm install -g vercel
   ```

2. Navigate to this folder in terminal:
   ```bash
   cd axiogrid-deploy
   ```

3. Run:
   ```bash
   vercel
   ```

4. Follow the prompts. Done!

---

### Option B: Deploy via GitHub + Vercel Dashboard

1. **Create a new GitHub repository:**
   - Go to https://github.com/new
   - Name it `axiogrid-website`
   - Keep it private or public (your choice)
   - Click "Create repository"

2. **Upload these files to GitHub:**
   - Click "uploading an existing file"
   - Drag both `index.html` and `vercel.json` into the upload area
   - Click "Commit changes"

3. **Connect to Vercel:**
   - Go to https://vercel.com/new
   - Click "Import" next to your `axiogrid-website` repo
   - Click "Deploy"
   - Wait ~30 seconds

4. **Your site is live!** You'll get a URL like `axiogrid-website.vercel.app`

---

## Connect Your Domain (axiogrid.ai)

### In Vercel:
1. Go to your project dashboard
2. Click "Settings" → "Domains"
3. Add `axiogrid.ai`
4. Vercel will show you DNS records to add

### In Namecheap:
1. Log into Namecheap → Domain List → Manage (axiogrid.ai)
2. Go to "Advanced DNS"
3. Delete existing records (or modify them)
4. Add the records Vercel shows you:
   - Type: `A` | Host: `@` | Value: `76.76.19.19`
   - Type: `CNAME` | Host: `www` | Value: `cname.vercel-dns.com`

5. Wait 5-10 minutes for DNS propagation
6. Visit axiogrid.ai - your new site is live! 🎉

---

## Files Included
- `index.html` - Your complete website (logo embedded)
- `vercel.json` - Vercel configuration
- `README.md` - This file
