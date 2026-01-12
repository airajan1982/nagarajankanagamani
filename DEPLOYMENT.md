# GitHub Pages Deployment Guide

## 🌐 Your Portfolio Website URL
Once configured, your site will be available at:
**https://airajan1982.github.io/nagarajankanagamani/**

---

## 📋 Quick Deployment Steps

### Method 1: Deploy from Current Branch (Fastest - 2 minutes)

1. Visit your repository: https://github.com/airajan1982/nagarajankanagamani

2. Click **Settings** (top navigation bar)

3. Click **Pages** in the left sidebar

4. Under "Build and deployment":
   - **Source**: Deploy from a branch
   - **Branch**: `claude/create-portfolio-website-zsRTS`
   - **Folder**: `/ (root)`
   - Click **Save**

5. Wait 1-2 minutes for deployment

6. Refresh the Pages settings page to see your live URL!

---

### Method 2: Deploy from Main Branch (Recommended for Production)

#### Step 1: Merge the Pull Request

1. Visit: https://github.com/airajan1982/nagarajankanagamani/pull/new/claude/create-portfolio-website-zsRTS

2. Click **"Create pull request"**

3. Add title: "Add professional portfolio website"

4. Click **"Create pull request"** again

5. Click **"Merge pull request"**

6. Click **"Confirm merge"**

#### Step 2: Enable GitHub Pages

1. Go to **Settings** → **Pages**

2. Under "Build and deployment":
   - **Source**: Deploy from a branch
   - **Branch**: `main`
   - **Folder**: `/ (root)`
   - Click **Save**

3. Wait 1-2 minutes for deployment

4. Your site will be live at: https://airajan1982.github.io/nagarajankanagamani/

---

## ✅ Verification Steps

After enabling GitHub Pages:

1. **Check deployment status:**
   - Go to repository → **Actions** tab
   - You'll see "pages build and deployment" workflow running
   - Wait for the green checkmark ✓

2. **Visit your site:**
   - Click on the URL shown in Settings → Pages
   - Or directly visit: https://airajan1982.github.io/nagarajankanagamani/

3. **Test the site:**
   - Check if all sections load properly
   - Test the dark mode toggle
   - Try the mobile menu (resize browser or use mobile)
   - Test navigation links

---

## 🔧 Troubleshooting

### Site shows 404 error
- Wait a few more minutes (first deployment takes longer)
- Check that you saved the correct branch in Pages settings
- Verify the branch has the `index.html` file

### Site doesn't update after changes
- Go to Actions tab and wait for deployment to complete
- Clear your browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Try incognito/private browsing mode

### CSS/styling looks broken
- This shouldn't happen as all CSS is embedded
- Check browser console for errors (F12)
- Verify you're viewing the correct URL

---

## 🎨 Customization Reminders

Before sharing your site, make sure to update:

- [ ] Your name and professional title (Hero section)
- [ ] Professional summary (About section)
- [ ] Work experience with actual dates and companies
- [ ] Skills and proficiency levels
- [ ] Education and certifications
- [ ] Contact information (email, LinkedIn)
- [ ] Projects/achievements
- [ ] Social media links in footer

See `README.md` for detailed customization instructions.

---

## 🌟 Custom Domain (Optional)

Want to use your own domain (e.g., nagarajankanagamani.com)?

1. **Buy a domain** from:
   - Namecheap
   - Google Domains
   - GoDaddy
   - Cloudflare

2. **Configure DNS:**
   Add these records in your domain provider:
   ```
   Type: A
   Host: @
   Value: 185.199.108.153

   Type: A
   Host: @
   Value: 185.199.109.153

   Type: A
   Host: @
   Value: 185.199.110.153

   Type: A
   Host: @
   Value: 185.199.111.153

   Type: CNAME
   Host: www
   Value: airajan1982.github.io
   ```

3. **Add custom domain in GitHub:**
   - Go to Settings → Pages
   - Under "Custom domain", enter your domain
   - Click Save
   - Wait for DNS check to complete

4. **Enable HTTPS:**
   - Check "Enforce HTTPS" option
   - Wait for certificate to be issued (~15 minutes)

---

## 📱 Sharing Your Portfolio

Once live, share your portfolio:

### Update LinkedIn Profile:
1. Go to your LinkedIn profile
2. Add website URL in the Contact section
3. Update your summary to mention your portfolio

### Update Resume:
Add your portfolio URL at the top of your resume

### Email Signature:
Include portfolio link in your professional email signature

### Social Media:
Share on Twitter, LinkedIn posts, etc.

---

## 📊 Analytics (Optional)

Want to track visitors? Add Google Analytics:

1. Create Google Analytics account: https://analytics.google.com

2. Get your Measurement ID (looks like G-XXXXXXXXXX)

3. Update `index.html` - add before `</head>`:
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

4. Commit and push changes

5. View analytics in Google Analytics dashboard

---

## 🚀 Need Help?

If you encounter issues:
1. Check the GitHub Pages documentation: https://docs.github.com/en/pages
2. Verify your repository is public (Pages requires public repos for free tier)
3. Check the Actions tab for deployment errors
4. Review the README.md for customization help

---

## 🎉 You're All Set!

Your professional portfolio is ready to impress recruiters and potential employers!

**Next steps:**
1. Enable GitHub Pages (see Method 1 or 2 above)
2. Customize content with your information
3. Share your portfolio URL everywhere!

Good luck with your job search! 🌟
