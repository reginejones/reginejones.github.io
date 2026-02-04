# Regine Jones - Portfolio Website

A modern, design-focused portfolio website built to showcase AI/ML engineering skills and projects. Designed to impress tech recruiters with stunning visuals and smooth animations.

## ✨ Features

- **Stunning Visual Design** - Dark theme with gradient accents and glassmorphism effects
- **Smooth Animations** - Scroll-triggered animations, typing effects, and parallax scrolling
- **Fully Responsive** - Looks great on all devices from mobile to desktop
- **Interactive Elements** - Project filtering, skill bars, cursor glow effects
- **Performance Optimized** - Lazy loading, CSS animations, minimal dependencies
- **SEO Ready** - Meta tags, Open Graph support, semantic HTML
- **Accessible** - Follows WCAG guidelines, respects reduced motion preferences
- **Easter Egg** - Try the Konami code! (↑↑↓↓←→←→BA)

## 🚀 Quick Start

### Option 1: View Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/reginejones/reginejones.github.io.git
   cd reginejones.github.io
   ```

2. **Open locally:**
   Simply open `index.html` in your browser, or use a local server:
   
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve
   ```

3. **Visit:** `http://localhost:8000`

### Option 2: Deploy to GitHub Pages

Follow the deployment instructions below to get your site live!

## 🎨 Customization

### Personal Information

Edit `index.html` to update:
- Name and title
- About section content
- Projects (update links, descriptions, metrics)
- Work experience
- Publications and awards
- Contact information and social links

### Styling

Modify `styles.css` to customize:
- **Colors**: Update CSS custom properties in `:root`
- **Typography**: Change font imports and `--font-primary`
- **Spacing**: Adjust `--section-padding` and `--container-width`

### Adding Your Photo

Replace the placeholder in the About section:

```html
<!-- Find this in index.html -->
<div class="image-placeholder">...</div>

<!-- Replace with: -->
<img src="assets/your-photo.jpg" alt="Regine Jones" />
```

### Typing Text

Edit the phrases in `script.js`:

```javascript
const phrases = [
    'AI/ML Engineer',
    'Deep Learning Researcher',
    // Add your own titles
];
```

## 📤 Deployment to GitHub Pages

### Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the **+** icon in the top right and select **New repository**
3. Name your repository: `reginejones.github.io`
   - *Important*: Replace `reginejones` with your actual GitHub username
4. Make it **Public**
5. Do **NOT** initialize with README, .gitignore, or license
6. Click **Create repository**

### Step 2: Push Your Code to GitHub

Open your terminal in the project folder and run:

```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit your changes
git commit -m "Initial commit: Regine Jones portfolio website"

# Rename branch to main
git branch -M main

# Add your GitHub repository as remote
# Replace YOUR_USERNAME with your actual GitHub username
git remote add origin https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io.git

# Push to GitHub
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Scroll down and click **Pages** in the left sidebar
4. Under **Source**, select:
   - **Branch**: `main`
   - **Folder**: `/ (root)`
5. Click **Save**

### Step 4: Access Your Live Site

Your site will be live at: `https://YOUR_USERNAME.github.io`

*Note: It may take a few minutes for the site to become available*

## 🔄 Updating Your Site

After making changes to your files:

```bash
# Add changed files
git add .

# Commit changes
git commit -m "Description of changes"

# Push to GitHub
git push
```

Your site will automatically update within a few minutes!

## 🌐 Alternative Deployment Options

### Netlify

1. Drag and drop the folder to [netlify.com/drop](https://netlify.com/drop)
2. Or connect your GitHub repo for continuous deployment

### Vercel

1. Install Vercel CLI: `npm i -g vercel`
2. Run: `vercel`
3. Follow the prompts

### Custom Domain

To use a custom domain with GitHub Pages:

1. Add a `CNAME` file to your repository with your domain:
   ```
   www.reginejones.com
   ```

2. Configure your domain's DNS settings:
   - Add a CNAME record pointing to `YOUR_USERNAME.github.io`

3. In GitHub repository settings → Pages → Custom domain, enter your domain

## 📁 Project Structure

```
reginejones.github.io/
├── index.html          # Main HTML file
├── styles.css          # All styling
├── script.js           # Interactivity & animations
├── README.md           # This file
└── assets/             # Images, resume, etc. (create as needed)
    ├── your-photo.jpg
    ├── resume.pdf
    └── og-image.png
```

## 🌐 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## ⚡ Performance Tips

- Compress images before adding to `assets/`
- Use WebP format for photos where supported
- Consider adding a service worker for offline support
- Optimize SVGs with [SVGO](https://github.com/svg/svgo)

## 📧 Contact Form Setup

The contact form currently simulates submission. To make it functional:

### Option 1: Formspree

```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

1. Sign up at [formspree.io](https://formspree.io)
2. Create a new form
3. Replace `YOUR_FORM_ID` with your actual form ID

### Option 2: Netlify Forms

```html
<form name="contact" netlify>
```

Works automatically when deployed to Netlify!

### Option 3: Custom Backend

Update `script.js` to POST to your API endpoint:

```javascript
const response = await fetch('YOUR_API_ENDPOINT', {
    method: 'POST',
    headers: {
        'Content-Type': 'application/json',
    },
    body: JSON.stringify(formData)
});
```

## 🎯 SEO Optimization

1. **Update Meta Tags** in `index.html`:
   ```html
   <meta name="description" content="Your custom description">
   <meta property="og:image" content="your-image-url">
   ```

2. **Create `sitemap.xml`** (optional but recommended)

3. **Add Google Analytics** (if desired):
   ```html
   <!-- Add to <head> section -->
   <script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
   ```

## 🐛 Troubleshooting

### Site not loading?
- Check that your repository name is exactly `YOUR_USERNAME.github.io`
- Wait a few minutes after pushing - deployment takes time
- Check GitHub Pages settings are correct

### Images not showing?
- Make sure image paths are correct
- Images should be in the `assets/` folder
- Use relative paths: `assets/image.jpg` not `/assets/image.jpg`

### Mobile menu not working?
- Check that `script.js` is loading correctly
- Open browser console for any JavaScript errors

## 📝 License

MIT License - Feel free to use and modify for your own portfolio!

## 🙏 Acknowledgments

- Fonts from [Google Fonts](https://fonts.google.com)
- Icons and emojis for visual elements
- Inspired by modern portfolio designs

## 💡 Tips for Success

1. **Keep it updated** - Regularly add new projects and achievements
2. **Personalize it** - Make it truly yours with custom colors and content
3. **Test thoroughly** - Check on different devices and browsers
4. **Get feedback** - Ask friends and colleagues for their input
5. **Iterate** - Continuously improve based on feedback

## 📞 Support

If you encounter any issues or have questions:
1. Check the [GitHub Issues](https://github.com/reginejones/reginejones.github.io/issues)
2. Review the troubleshooting section above
3. Open a new issue with details about your problem
