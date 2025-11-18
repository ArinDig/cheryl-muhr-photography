# Deployment Guide 🚀

Your website is ready to deploy! Here are two quick methods:

---

## Method 1: GitHub + Vercel (Recommended)

This creates a nice workflow where any future changes you push to GitHub will automatically update your site.

### Step 1: Create GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Name your repository: `cheryl-muhr-photography` (or any name you like)
3. Keep it **Public** (or Private - both work with Vercel)
4. **Don't** initialize with README, .gitignore, or license (we already have those)
5. Click **Create repository**

### Step 2: Push Your Code to GitHub

GitHub will show you commands. Use these in your terminal:

```bash
cd "/Users/arinbrown/Documents/Arin Digital Innovations/CMP/Cursor_CMP"
git remote add origin https://github.com/YOUR_USERNAME/cheryl-muhr-photography.git
git branch -M main
git push -u origin main
```

Replace `YOUR_USERNAME` with your actual GitHub username.

### Step 3: Deploy to Vercel

1. Go to [vercel.com](https://vercel.com) and sign in
2. Click **Add New** → **Project**
3. Import your GitHub repository (you may need to authorize Vercel to access your GitHub)
4. Find `cheryl-muhr-photography` and click **Import**
5. Vercel will auto-detect the settings:
   - **Framework Preset**: Other (or leave as detected)
   - **Root Directory**: ./
   - **Build Command**: (leave empty)
   - **Output Directory**: (leave empty)
6. Click **Deploy**

**That's it!** Vercel will give you a URL like:
- `cheryl-muhr-photography.vercel.app`
- Or `your-project-name-xxx.vercel.app`

---

## Method 2: Direct Vercel Deploy (Fastest)

If you want to skip GitHub for now and deploy instantly:

### Using Vercel CLI

1. **Install Vercel CLI** (if you haven't):
   ```bash
   npm install -g vercel
   ```

2. **Deploy**:
   ```bash
   cd "/Users/arinbrown/Documents/Arin Digital Innovations/CMP/Cursor_CMP"
   vercel
   ```

3. **Follow the prompts**:
   - Login to Vercel (if not already)
   - Answer the questions (defaults are usually fine)
   - Get your preview URL instantly!

### Using Vercel Dashboard (No CLI needed)

1. Go to [vercel.com/new](https://vercel.com/new)
2. Choose **"Deploy from a template"** → or scroll down to **"Import Git Repository"**
3. If you see "Deploy from the CLI", use the CLI method above
4. You can also drag & drop your project folder in some cases

---

## Quick Commands Reference

All commands assume you're in the project directory:

```bash
# Navigate to project
cd "/Users/arinbrown/Documents/Arin Digital Innovations/CMP/Cursor_CMP"

# Check git status
git status

# View remote URLs
git remote -v

# Make changes and commit
git add .
git commit -m "Description of changes"
git push

# Deploy with Vercel CLI
vercel --prod
```

---

## After Deployment

### Testing on Different Devices

Once deployed, you'll get a URL like:
- `https://cheryl-muhr-photography.vercel.app`

Open this URL on:
- ✅ Your phone
- ✅ Your tablet  
- ✅ Your laptop
- ✅ Share with friends for feedback

### Domain Setup (Optional)

Both GitHub Pages and Vercel support custom domains:

1. **On Vercel Dashboard**:
   - Go to your project
   - Click **Settings** → **Domains**
   - Add your custom domain (like `cherylmuhrphotography.com`)
   - Follow the DNS setup instructions

2. **Domain Providers** (where to buy):
   - [Namecheap](https://namecheap.com)
   - [Google Domains](https://domains.google)
   - [Cloudflare](https://cloudflare.com) (also includes DNS)

---

## Automatic Updates

With GitHub + Vercel connected:
1. Make changes locally
2. Commit: `git add . && git commit -m "Updated photos"`
3. Push: `git push`
4. Vercel automatically deploys! ✨

Your preview URL updates in ~30 seconds.

---

## Need Help?

If you encounter any issues:
- Check that git remote is set: `git remote -v`
- Make sure you're on the main branch: `git branch`
- Verify Vercel has access to your GitHub repo in settings

The site is 100% static HTML/CSS/JS, so it will work on any hosting platform!

