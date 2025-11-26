# Academic Website Template

A modern, responsive academic website template perfect for researchers, professors, and academics. This template is designed to work seamlessly with GitHub Pages.

## 🌟 Features

- **Modern & Responsive Design**: Looks great on all devices (desktop, tablet, mobile)
- **Easy to Customize**: Simple HTML structure with clear sections
- **Professional Layout**: Includes all essential sections for an academic website
- **Smooth Animations**: Elegant scroll animations and transitions
- **Fast Loading**: Optimized for performance
- **SEO Friendly**: Proper meta tags and semantic HTML

## 📋 Sections Included

1. **Home/Hero**: Eye-catching introduction with profile picture and social links
2. **About**: Biography, awards, experience, and education
3. **Research**: Showcase your research areas and projects
4. **Publications**: Display your academic publications by year
5. **Teaching**: List courses and mentoring information
6. **Contact**: Office hours, email, and location information

## 🚀 Getting Started

### Option 1: Deploy to GitHub Pages

1. **Create a new repository**:
   - Go to GitHub and create a new repository named `username.github.io` (replace `username` with your GitHub username)
   - For a project page, name it anything you like (e.g., `my-academic-website`)

2. **Upload these files**:
   - Upload all the files from this template to your repository

3. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Under "Source", select the branch (usually `main`)
   - Click Save

4. **Access your site**:
   - For user site: `https://username.github.io`
   - For project site: `https://username.github.io/repository-name`

### Option 2: Local Development

1. **Clone or download** this repository
2. **Open `index.html`** in your web browser
3. **Edit the files** to customize your website
4. **Test locally** before deploying

## ✏️ Customization Guide

### 1. Update Personal Information

Open `index.html` and replace all placeholder text marked with `[brackets]`:

- `[Your Name]` - Your full name
- `[Your Title/Position]` - Your current position
- `[Your Department]` - Your department name
- `[Your University]` - Your institution name
- Update email addresses, social media links, etc.

### 2. Replace Profile Picture

Replace the placeholder image URL in the hero section:
```html
<img src="https://via.placeholder.com/300x300" alt="Profile Picture">
```

Change to:
```html
<img src="images/profile.jpg" alt="Your Name">
```

Then add your profile picture to an `images` folder.

### 3. Update Publications

In the Publications section, replace the sample publications with your own:
- Update author names (bold your name)
- Add paper titles
- Include venue and year
- Add links to PDFs, code, project pages, etc.

### 4. Customize Colors

Edit `css/style.css` and modify the CSS variables at the top:

```css
:root {
    --primary-color: #2c3e50;      /* Main dark color */
    --secondary-color: #3498db;    /* Accent blue color */
    --accent-color: #e74c3c;       /* Highlight red color */
    /* Adjust these to match your preferences */
}
```

### 5. Add More Sections (Optional)

You can add additional sections like:
- Blog
- Software/Tools
- Media Coverage
- Awards & Honors (expanded)
- Talks & Presentations

## 📁 File Structure

```
Omar_website/
│
├── index.html          # Main HTML file
├── css/
│   └── style.css      # Stylesheet
├── js/
│   └── script.js      # JavaScript for interactivity
├── images/            # (Create this folder for images)
│   └── profile.jpg    # Your profile picture
└── README.md          # This file
```

## 🎨 Icons

This template uses [Font Awesome 6](https://fontawesome.com/) for icons. You can:
- Browse available icons at [fontawesome.com/icons](https://fontawesome.com/icons)
- Replace existing icons by changing the class names (e.g., `fa-envelope`, `fa-github`)

## 📱 Mobile Responsive

The template is fully responsive and includes:
- Hamburger menu for mobile devices
- Flexible grid layouts that adapt to screen size
- Touch-friendly navigation

## 🔧 Browser Compatibility

Works on all modern browsers:
- Chrome
- Firefox
- Safari
- Edge

## 📝 Tips for Content

### Writing Your Bio
- Keep it concise but informative
- Highlight your main research interests
- Mention key achievements and affiliations
- Update regularly

### Publications Section
- List most recent first
- Bold your name in author lists
- Include links to papers when possible
- Consider adding citation counts or impact

### Research Section
- Use clear, accessible language
- Explain the significance of your work
- Include visuals if possible

## 🤝 Support

If you encounter any issues or have questions:
1. Check that all files are in the correct directories
2. Verify that file names match exactly (case-sensitive)
3. Test in a different browser
4. Clear your browser cache

## 📄 License

This template is free to use and modify for your personal academic website. No attribution required, but appreciated!

## 🌐 Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)
- [Font Awesome Icons](https://fontawesome.com/icons)
- [CSS Color Picker](https://htmlcolorcodes.com/)

## ✨ Credits

Created with ❤️ for the academic community.

---

**Good luck with your academic website!** 🎓

