# 🌿 Garden of Edyn Photography

A beautiful, responsive photo portfolio website built for GitHub Pages. Perfect for showcasing photography work across multiple categories.

## 📸 Features

- **Responsive Design**: Looks great on desktop, tablet, and mobile devices
- **Three Portfolio Categories**: 
  - Landscapes
  - Close-Ups
  - Product Promotions
- **Lightbox Gallery**: Click any photo to view in full-screen with keyboard navigation
- **Smooth Animations**: Scroll effects and fade-in animations
- **Mobile Navigation**: Hamburger menu for mobile devices
- **SEO Optimized**: Meta tags and semantic HTML

## 🚀 Quick Start

### 1. Add Your Photos

Create the following folder structure in your project:

```
photo-portfolio/
├── images/
│   ├── landscapes/
│   │   ├── landscape1.jpg
│   │   ├── landscape2.jpg
│   │   ├── landscape-thumb.jpg (for home page)
│   │   └── ...
│   ├── closeups/
│   │   ├── closeup1.jpg
│   │   ├── closeup2.jpg
│   │   ├── closeup-thumb.jpg (for home page)
│   │   └── ...
│   └── products/
│       ├── product1.jpg
│       ├── product2.jpg
│       ├── product-thumb.jpg (for home page)
│       └── ...
```

**Image Recommendations:**
- **Gallery photos**: 1200-2000px wide, optimized for web
- **Thumbnail photos** (for home page): 800px wide minimum
- Format: JPG or PNG
- Compress images for faster loading (use tools like TinyPNG or ImageOptim)

### 2. Deploy to GitHub Pages

#### Method 1: Through GitHub Website

1. Create a new repository on GitHub (e.g., `photo-portfolio`)
2. Upload all files to the repository
3. Go to **Settings** → **Pages**
4. Under "Source", select the `main` branch
5. Click **Save**
6. Your site will be live at `https://yourusername.github.io/photo-portfolio/`

#### Method 2: Using Git Commands

```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit changes
git commit -m "Initial commit - Garden of Edyn Photography"

# Add remote repository (replace with your repository URL)
git remote add origin https://github.com/yourusername/photo-portfolio.git

# Push to GitHub
git branch -M main
git push -u origin main

# Enable GitHub Pages in repository settings
```

### 3. Custom Domain (Optional)

1. Purchase a domain from a domain registrar
2. In your GitHub repository, go to **Settings** → **Pages**
3. Enter your custom domain
4. Add DNS records from your domain registrar:
   - Add a CNAME record pointing to `yourusername.github.io`

## 🎨 Customization

### Change Colors

Edit the CSS variables in `styles.css`:

```css
:root {
    --primary-color: #2c3e50;     /* Main dark color */
    --secondary-color: #e74c3c;   /* Accent color (red) */
    --accent-color: #3498db;      /* Blue accent */
}
```

### Update Site Name

Replace "Garden of Edyn" with your site name in:
- `index.html` (line 7, 24, 35)
- `landscapes.html` (line 7, 16)
- `closeups.html` (line 7, 16)
- `products.html` (line 7, 16)

### Add More Photos

1. Add image files to the appropriate folder
2. Edit the corresponding HTML file (e.g., `landscapes.html`)
3. Copy an existing photo item and update the image source and caption:

```html
<div class="photo-item">
    <img src="images/landscapes/your-photo.jpg" alt="Description" loading="lazy">
    <div class="photo-caption">Your Caption</div>
</div>
```

### Change Hero Background

In `styles.css`, line 227, replace the background image URL:

```css
.hero {
    background-image: url('your-image-url.jpg');
}
```

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## 🛠️ Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Modern styling with Grid and Flexbox
- **JavaScript**: Vanilla JS for interactions
- **Google Fonts**: Playfair Display & Raleway

## 📄 File Structure

```
photo-portfolio/
├── index.html              # Home page
├── landscapes.html         # Landscapes gallery
├── closeups.html          # Close-ups gallery
├── products.html          # Products gallery
├── styles.css             # All styles
├── script.js              # JavaScript functionality
├── README.md              # This file
└── images/                # Your photos folder
    ├── landscapes/
    ├── closeups/
    └── products/
```

## 💡 Tips for Best Results

1. **Optimize Images**: Compress images before uploading to improve load times
2. **Consistent Sizing**: Try to keep photos in similar aspect ratios within each category
3. **High Quality**: Use high-resolution photos (but web-optimized)
4. **Alt Text**: Update alt text for accessibility and SEO
5. **Regular Updates**: Add new photos regularly to keep your portfolio fresh

## 🐛 Troubleshooting

**Images not showing?**
- Check that image paths are correct
- Ensure images are uploaded to the correct folders
- Verify image file names match exactly (case-sensitive)

**Lightbox not working?**
- Make sure `script.js` is properly linked
- Check browser console for errors
- Clear browser cache and reload

**Site not deploying?**
- Verify GitHub Pages is enabled in repository settings
- Check that the source branch is correct
- Wait a few minutes for changes to propagate

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🌟 Credits

Created as a photography portfolio project. Feel free to use and modify for your own portfolio!

---

**Need help?** Check the [GitHub Pages documentation](https://docs.github.com/en/pages) or open an issue in this repository.

Happy showcasing! 📸✨