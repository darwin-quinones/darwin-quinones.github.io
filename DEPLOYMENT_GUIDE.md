# 🚀 GitHub Pages Deployment Guide

This guide will walk you through deploying your portfolio to GitHub Pages, making it accessible at `https://yourusername.github.io/portfolio` or `https://yourusername.github.io` (if using a user site).

## 📋 Prerequisites

- GitHub account ([Sign up here](https://github.com/signup))
- Git installed on your computer ([Download here](https://git-scm.com/downloads))
- Your portfolio files ready

## 🎯 Deployment Options

### Option 1: User/Organization Site (Recommended)
Your portfolio will be at: `https://yourusername.github.io`

### Option 2: Project Site
Your portfolio will be at: `https://yourusername.github.io/portfolio`

---

## 🚀 Step-by-Step Deployment

### Step 1: Create a GitHub Repository

1. **Go to GitHub** and sign in
2. **Click the "+" icon** in the top right corner
3. **Select "New repository"**

#### For Option 1 (User Site):
- Repository name: `yourusername.github.io` (replace with your actual username)
- Example: If your username is "darwinquinones", name it `darwinquinones.github.io`

#### For Option 2 (Project Site):
- Repository name: `portfolio` (or any name you prefer)

4. **Settings**:
   - ✅ Set to **Public**
   - ❌ Don't initialize with README (we already have one)
   - Click **"Create repository"**

### Step 2: Initialize Git in Your Project

Open PowerShell or Command Prompt in your portfolio folder and run:

```powershell
# Navigate to your portfolio folder (if not already there)
cd "c:\Users\darwi\Desktop\Desktop\projects\my projects\porfolio"

# Initialize git repository
git init

# Add all files
git add .

# Create your first commit
git commit -m "Initial commit: Professional portfolio website"
```

### Step 3: Connect to GitHub

Replace `yourusername` with your GitHub username:

#### For User Site:
```powershell
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git branch -M main
git push -u origin main
```

#### For Project Site:
```powershell
git remote add origin https://github.com/yourusername/portfolio.git
git branch -M main
git push -u origin main
```

**Note**: You'll be prompted to enter your GitHub credentials.

### Step 4: Enable GitHub Pages

1. **Go to your repository** on GitHub
2. **Click "Settings"** tab
3. **Click "Pages"** in the left sidebar
4. Under **"Source"**:
   - Select branch: `main`
   - Select folder: `/ (root)`
   - Click **"Save"**

5. **Wait a few minutes** for GitHub to build your site
6. **Refresh the page** - you'll see: "Your site is live at..."

### Step 5: Visit Your Live Site! 🎉

- **User Site**: `https://yourusername.github.io`
- **Project Site**: `https://yourusername.github.io/portfolio`

---

## 🔄 Making Updates

After making changes to your portfolio:

```powershell
# Add all changes
git add .

# Commit with a descriptive message
git commit -m "Update: Description of your changes"

# Push to GitHub
git push origin main
```

Your site will automatically update in a few minutes!

---

## 🎨 Customization Checklist

Before deploying, make sure you've customized:

### Essential Updates:
- [ ] Replace profile images with your actual photos
- [ ] Update all personal information (name, email, phone, location)
- [ ] Update social media links (LinkedIn, GitHub)
- [ ] Replace resume PDF with your own
- [ ] Update project descriptions and images
- [ ] Verify all links work correctly

### Optional Enhancements:
- [ ] Add real project screenshots
- [ ] Update tech stack based on your skills
- [ ] Customize color scheme if desired
- [ ] Add your own projects to replace placeholders
- [ ] Add Google Analytics (see below)

---

## 📊 Adding Google Analytics (Optional)

1. **Create a Google Analytics account** at [analytics.google.com](https://analytics.google.com)
2. **Get your tracking ID** (starts with "G-" or "UA-")
3. **Add to your `index.html`** before the closing `</head>` tag:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

---

## 🌐 Using a Custom Domain (Optional)

Want to use your own domain like `darwinquinones.com`?

### Step 1: Buy a Domain
Purchase from: [Namecheap](https://www.namecheap.com), [Google Domains](https://domains.google), or [GoDaddy](https://www.godaddy.com)

### Step 2: Configure DNS
In your domain provider's settings, add these DNS records:

```
Type    Name    Value
A       @       185.199.108.153
A       @       185.199.109.153
A       @       185.199.110.153
A       @       185.199.111.153
CNAME   www     yourusername.github.io
```

### Step 3: Configure GitHub
1. Go to repository **Settings > Pages**
2. Under **"Custom domain"**, enter: `yourdomain.com`
3. Click **"Save"**
4. Check **"Enforce HTTPS"** (wait 24 hours if not available immediately)

---

## 🔧 Troubleshooting

### Site not loading?
- Wait 5-10 minutes after enabling GitHub Pages
- Check that `index.html` is in the root folder
- Verify the repository is public
- Clear your browser cache

### Images not showing?
- Check image paths are correct
- Ensure images are committed to the repository
- Use relative paths, not absolute paths

### CSS/JS not loading?
- Verify file names match exactly (case-sensitive)
- Check file paths in `index.html`
- Clear browser cache and refresh

### 404 Error?
- Ensure repository name is correct for user sites
- Check GitHub Pages is enabled in settings
- Verify you're using the correct URL

---

## 📱 Testing Checklist

Before sharing your portfolio:

- [ ] Test on multiple browsers (Chrome, Firefox, Safari, Edge)
- [ ] Test on mobile devices
- [ ] Check all links work
- [ ] Verify contact form opens email client
- [ ] Test navigation smooth scrolling
- [ ] Verify animations work smoothly
- [ ] Check page load speed
- [ ] Test on different screen sizes

---

## 🎯 Next Steps

1. **Share your portfolio!**
   - Add link to LinkedIn profile
   - Include in resume
   - Share on social media
   - Add to email signature

2. **Monitor traffic**
   - Set up Google Analytics
   - Track visitor behavior
   - See which projects get the most attention

3. **Keep it updated**
   - Add new projects regularly
   - Update work experience
   - Refresh skills and technologies
   - Update resume periodically

---

## 🆘 Need Help?

- **GitHub Pages Docs**: [docs.github.com/pages](https://docs.github.com/pages)
- **Git Documentation**: [git-scm.com/doc](https://git-scm.com/doc)
- **Web Development**: [developer.mozilla.org](https://developer.mozilla.org)

---

## 📧 Support

If you run into issues:
1. Check the troubleshooting section above
2. Search on [Stack Overflow](https://stackoverflow.com)
3. Check [GitHub Community](https://github.community)

---

**Good luck with your job search!** 🚀

Your professional portfolio is a powerful tool for landing your next great opportunity. Keep it updated and share it proudly!

*Last Updated: February 2025*
