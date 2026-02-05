# Luxury Jewelry Website

A sophisticated, responsive website for a luxury jewelry business, designed to connect with potential sellers and high-end clients.

## Features

- **Elegant Design**: Premium aesthetic with gold accents and sophisticated typography
- **Fully Responsive**: Works seamlessly on desktop, tablet, and mobile devices
- **Smooth Animations**: Professional scroll effects and interactive elements
- **Optimized Performance**: Fast loading and smooth interactions
- **GitHub Pages Ready**: Can be deployed immediately to GitHub Pages

## Sections

1. **Hero**: Eye-catching landing section with call-to-action buttons
2. **About**: Company story and statistics
3. **Services**: Overview of offerings for clients and artisans
4. **Gallery**: Showcase of jewelry collections
5. **Contact**: Contact form and information for partnerships

## Customization Guide

### 1. Update Logo and Brand Name

Replace `LUXE JEWELS` in `index.html`:
- Line 18: `<span class="logo-text">YOUR BRAND NAME</span>`
- Line 241: Footer logo
- Update the diamond symbol `◆` with your logo image

### 2. Add Your Logo Image

Replace the placeholder diamond icon:
```html
<div class="logo">
    <img src="logo.png" alt="Your Brand" class="logo-img">
    <span class="logo-text">YOUR BRAND NAME</span>
</div>
```

### 3. Update Contact Information

In `index.html`, update:
- Email address (line 177)
- Phone number (line 186)

### 4. Add Real Images

Replace the SVG placeholders in the gallery section:
```html
<div class="gallery-item">
    <img src="images/ring-collection.jpg" alt="Ring Collection">
    <div class="gallery-overlay">
        <h4>Classic Rings</h4>
    </div>
</div>
```

### 5. Customize Colors

In `styles.css`, update the CSS variables:
```css
:root {
    --primary-gold: #D4AF37;  /* Your brand color */
    --dark-bg: #0a0a0a;       /* Background color */
    /* ... */
}
```

### 6. Connect Contact Form

The form currently logs to console. To make it functional:
- Use a service like Formspree, Netlify Forms, or EmailJS
- Or connect to your own backend API

Example with Formspree:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### 7. Add Social Media Links

Update footer social links (lines 244-246):
```html
<li><a href="https://instagram.com/yourbrand" target="_blank">Instagram</a></li>
```

## Deployment to GitHub Pages

1. Push your code to GitHub:
```bash
git add .
git commit -m "Initial website commit"
git push origin main
```

2. Go to your repository settings on GitHub
3. Navigate to "Pages" in the left sidebar
4. Under "Source", select "main" branch and "/ (root)" folder
5. Click "Save"
6. Your site will be published at: `https://yourusername.github.io/yourrepo`

## Custom Domain Setup

To connect your custom domain:

1. In your repository settings → Pages → Custom domain, enter your domain
2. In your domain registrar, add these DNS records:
   - For apex domain (example.com):
     ```
     A     185.199.108.153
     A     185.199.109.153
     A     185.199.110.153
     A     185.199.111.153
     ```
   - For www subdomain:
     ```
     CNAME    yourusername.github.io
     ```
3. Wait for DNS propagation (can take up to 24 hours)
4. Enable HTTPS in GitHub Pages settings

## File Structure

```
webpage/
├── index.html          # Main HTML file
├── styles.css          # All styling
├── script.js           # JavaScript functionality
└── README.md          # This file
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Future Enhancements

Consider adding:
- Image gallery lightbox
- Blog section
- Testimonials
- Multi-language support
- Analytics tracking (Google Analytics)
- Cookie consent banner (if needed for GDPR)

## License

All rights reserved.
