# Deployment Guide for GitHub Pages

This guide will walk you through deploying your academic website to GitHub Pages step by step.

## Quick Start (5 minutes)

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the **"+"** button in the top right → **"New repository"**
3. Choose a repository name:
   - For a personal site: `yourusername.github.io` (e.g., `johnsmith.github.io`)
   - For a project site: any name (e.g., `academic-website`)
4. Make it **Public**
5. **Don't** initialize with README (we already have files)
6. Click **"Create repository"**

### Step 2: Upload Your Files

**Option A: Using GitHub Web Interface** (Easiest)
1. On your new repository page, click **"uploading an existing file"**
2. Drag and drop ALL files from your `Omar_website` folder
3. Write a commit message: "Initial website commit"
4. Click **"Commit changes"**

**Option B: Using Git Command Line**
```bash
# Navigate to your website folder
cd /Users/sbhar/Downloads/Omar_website

# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial website commit"

# Add your GitHub repository as remote
git remote add origin https://github.com/yourusername/your-repo-name.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Click **Pages** (left sidebar)
4. Under "Source":
   - Branch: Select **main**
   - Folder: Select **/ (root)**
5. Click **Save**

### Step 4: Wait & Access Your Site

- GitHub will build your site (takes 1-2 minutes)
- Your site will be available at:
  - Personal: `https://yourusername.github.io`
  - Project: `https://yourusername.github.io/repository-name`

## Customization Checklist

Before publishing, make sure to update:

### Essential Updates ✅

- [ ] Replace `[Your Name]` with your actual name
- [ ] Update `[Your Title/Position]`
- [ ] Update `[Your Department]` and `[Your University]`
- [ ] Replace profile picture URL or add your photo to `images/` folder
- [ ] Update email address
- [ ] Update social media links (GitHub, Google Scholar, LinkedIn, Twitter)
- [ ] Add your actual publications
- [ ] Update research descriptions
- [ ] Add your courses
- [ ] Update contact information (office, phone, address)
- [ ] Update office hours

### Optional Updates ⚙️

- [ ] Change color scheme in `css/style.css`
- [ ] Add Google Analytics (if desired)
- [ ] Add custom domain (if you have one)
- [ ] Optimize images for web
- [ ] Add CV/Resume PDF download link

## Adding Your Profile Picture

1. Create an `images` folder in your website directory
2. Add your profile picture (e.g., `profile.jpg`)
3. Update `index.html`:

```html
<!-- Change this: -->
<img src="https://via.placeholder.com/300x300" alt="Profile Picture">

<!-- To this: -->
<img src="images/profile.jpg" alt="Your Name">
```

4. Recommended image size: 500x500 pixels, under 200KB

## Adding a PDF CV

1. Add your CV file to your repository (e.g., `cv.pdf`)
2. Add a download link in your HTML:

```html
<a href="cv.pdf" class="pub-link" download>
    <i class="fas fa-file-pdf"></i> Download CV
</a>
```

## Custom Domain (Optional)

If you own a domain name:

1. Create a file named `CNAME` (no extension) in your repository
2. Add your domain name to the file:
   ```
   www.yourname.com
   ```
3. Configure your domain's DNS settings:
   - Add a CNAME record pointing to `yourusername.github.io`
4. Wait for DNS propagation (can take up to 48 hours)

## Updating Your Website

### Using GitHub Web Interface:
1. Navigate to the file you want to edit
2. Click the pencil icon (Edit)
3. Make changes
4. Scroll down and click "Commit changes"
5. Wait 1-2 minutes for changes to appear

### Using Git:
```bash
# Make your changes to files
# Then:
git add .
git commit -m "Update description of changes"
git push
```

## Troubleshooting

### My site shows a 404 error
- Wait 2-3 minutes after enabling GitHub Pages
- Check that `index.html` is in the root directory
- Verify GitHub Pages is enabled in Settings → Pages

### Images aren't showing
- Check file paths are correct
- Use relative paths (e.g., `images/photo.jpg`, not `/images/photo.jpg`)
- File names are case-sensitive

### CSS/Styling not working
- Clear your browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Check that `css/style.css` is in the correct folder
- Verify the path in `index.html`: `<link rel="stylesheet" href="css/style.css">`

### Changes not appearing
- GitHub Pages can take 1-5 minutes to rebuild
- Clear browser cache
- Try incognito/private browsing mode

## Testing Locally

To test your site on your computer before publishing:

1. Simply open `index.html` in your web browser
2. Or use a local server:

```bash
# Python 3
python3 -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Then visit: http://localhost:8000
```

## Performance Tips

- **Optimize images**: Use tools like [TinyPNG](https://tinypng.com/) to compress images
- **Use WebP format**: For better compression (convert JPG/PNG to WebP)
- **Minify CSS/JS**: Use online tools to minify code (optional)
- **Enable caching**: GitHub Pages automatically handles this

## SEO Tips

1. Update meta description in `index.html`:
   ```html
   <meta name="description" content="Your custom description">
   ```

2. Add keywords:
   ```html
   <meta name="keywords" content="your, research, keywords">
   ```

3. Update the page title:
   ```html
   <title>Dr. Your Name - Researcher in Your Field</title>
   ```

## Security & Privacy

- Don't include personal phone numbers if you're concerned about privacy
- Use university email addresses
- Be cautious about sharing office hours publicly
- Consider using a contact form instead of direct email

## Maintenance

### Regular Updates (Recommended):
- [ ] Update publications when new papers are published
- [ ] Add new courses each semester
- [ ] Update profile picture periodically
- [ ] Keep research descriptions current
- [ ] Update awards and honors

### Annual Review:
- [ ] Review all content for accuracy
- [ ] Check all links still work
- [ ] Update copyright year
- [ ] Refresh biography

## Getting Help

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Community Forum](https://github.community/)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/github-pages)

## Advanced Features (Optional)

### Add Google Analytics
1. Get your tracking ID from Google Analytics
2. Add before `</head>` in `index.html`:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

### Add a Blog Section
Consider integrating:
- Jekyll blog (native GitHub Pages support)
- Medium or Substack (external link)
- Static blog generator

---

**Need help?** Feel free to open an issue on the GitHub repository or consult the documentation links above.

Good luck with your academic website! 🚀

