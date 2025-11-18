# Cheryl Muhr Photography Website

A clean, modern, and elegant photography website for Cheryl Muhr Photography based in Austin, TX.

## 🌟 Features

- **Responsive Design** - Looks beautiful on all devices (desktop, tablet, mobile)
- **Clean & Elegant Style** - White background with sophisticated typography
- **Easy Image Management** - Simple system for replacing placeholder images with your photos
- **Smooth Navigation** - Intuitive menu with smooth scrolling
- **Contact Form** - Built-in contact form for client inquiries
- **Portfolio Sections** - Dedicated galleries for Families and Seniors

## 📁 Project Structure

```
Cursor_CMP/
├── index.html          # Main HTML file with all sections
├── styles.css          # All styling and responsive design
├── script.js           # Interactive features (navigation, form)
├── images/             # Folder for all photography images
│   └── README.md       # Detailed guide for image management
└── README.md           # This file
```

## 🚀 Getting Started

### Option 1: Open Directly in Browser
1. Simply double-click `index.html` to open it in your default browser
2. The website will work with placeholder images from Unsplash

### Option 2: Use a Local Server (Recommended)
For the best experience, especially when testing:

1. **Using Python** (if you have Python installed):
   ```bash
   # Python 3
   python -m http.server 8000
   # Or Python 2
   python -m SimpleHTTPServer 8000
   ```
   Then open `http://localhost:8000` in your browser

2. **Using VS Code Live Server**:
   - Install the "Live Server" extension
   - Right-click on `index.html`
   - Select "Open with Live Server"

## 📸 Replacing Images with Your Photos

See the detailed guide in `images/README.md` for step-by-step instructions.

**Quick Summary:**
1. Save your photos with these exact names in the `images/` folder:
   - `about.jpg` (your professional portrait)
   - `family-1.jpg` through `family-6.jpg` (family portfolio)
   - `senior-1.jpg` through `senior-6.jpg` (senior portfolio)

2. Once you've added your images, update the image paths in `index.html`:
   - Change from: `https://images.unsplash.com/...`
   - Change to: `images/your-filename.jpg`

## ✏️ Customizing Content

### Update Text Content
Open `index.html` and search for the section you want to edit:
- **Hero Section**: Line ~32-40
- **About Section**: Line ~45-60
- **Family Section**: Line ~64-92
- **Senior Section**: Line ~96-126
- **Contact Section**: Line ~130-185

### Change Colors & Styling
Open `styles.css` and modify the CSS variables at the top (lines 1-15):
```css
:root {
    --primary-color: #2c2c2c;      /* Main text color */
    --secondary-color: #6b6b6b;    /* Secondary text */
    --accent-color: #d4a574;       /* Accent color (currently unused) */
    /* ... */
}
```

### Modify Fonts
The site uses Google Fonts:
- **Headings**: Cormorant Garamond (elegant serif)
- **Body Text**: Montserrat (clean sans-serif)

To change fonts, update the Google Fonts link in `index.html` (lines 7-9) and the CSS variables in `styles.css`.

## 📧 Setting Up the Contact Form

The contact form currently shows an alert when submitted. To make it functional:

### Option 1: Formspree (Free & Easy)
1. Sign up at [Formspree.io](https://formspree.io/)
2. Create a new form and get your form endpoint
3. In `index.html`, update the form tag:
   ```html
   <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
4. Remove or comment out the JavaScript form handler in `script.js`

### Option 2: Netlify Forms (If hosting on Netlify)
1. Add `netlify` attribute to the form tag:
   ```html
   <form class="contact-form" name="contact" netlify>
   ```
2. Deploy to Netlify - forms will work automatically!

### Option 3: Custom Backend
Connect to your own backend API by modifying the form submission handler in `script.js`.

## 🌐 Hosting Your Website

### Free Hosting Options:

**1. Netlify** (Recommended)
- Drag and drop your folder to [Netlify Drop](https://app.netlify.com/drop)
- Or connect your GitHub repository for automatic deployments
- Free SSL, custom domain support

**2. GitHub Pages**
- Create a GitHub repository
- Push your code
- Enable GitHub Pages in Settings
- Your site will be at `yourusername.github.io/repo-name`

**3. Vercel**
- Import your project from GitHub
- Automatic deployments on every push
- Free SSL and custom domains

### Custom Domain Setup
Once hosted, you can connect a custom domain like `cherylmuhrphotography.com`:
1. Purchase a domain from providers like Namecheap, GoDaddy, or Google Domains
2. Follow your hosting provider's instructions to connect the domain
3. Most hosting platforms provide simple guides for this

## 📱 Browser Compatibility

This website works on:
- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🎨 Design Credits

- Inspired by [Leigh Carolyn Photography](https://leighcarolyn.com)
- Stock photos from [Unsplash](https://unsplash.com)
- Fonts from [Google Fonts](https://fonts.google.com)

## 📞 Need Help?

If you need assistance with:
- Customizing the design
- Adding new sections
- Setting up hosting
- Connecting the contact form
- SEO optimization

Feel free to reach out for support!

## 📝 License

This website was created for Cheryl Muhr Photography. All photography content rights belong to Cheryl Muhr.

---

**Built with ❤️ for Cheryl Muhr Photography**

