# Image Management Guide

## Quick Start: Replacing Placeholder Images

This website is set up to make it **super easy** to replace the placeholder images with your actual photography. Simply follow these steps:

### Step 1: Prepare Your Images

Save your photos with these exact filenames in the `images/` folder:

#### About Section
- `about.jpg` - Your professional portrait (recommended size: 600px × 800px)

#### Family Portfolio
- `family-1.jpg` through `family-6.jpg` (recommended size: 800px × 1000px each)

#### Senior Portfolio
- `senior-1.jpg` through `senior-6.jpg` (recommended size: 800px × 1000px each)

### Step 2: Image Specifications

For best results, follow these guidelines:

**File Format:** JPG or PNG
**Aspect Ratio:** 
- Portfolio images: 4:5 ratio (e.g., 800px × 1000px)
- About image: 3:4 ratio (e.g., 600px × 800px)

**File Size:** Optimize images to 200-500KB each for fast loading
- Use tools like [TinyPNG](https://tinypng.com/) or [ImageOptim](https://imageoptim.com/)

### Step 3: Replace the Files

1. Save your edited/optimized photos with the exact filenames listed above
2. Drop them into the `images/` folder (replacing the placeholders)
3. Refresh your website - done! Your images will automatically appear

## Using Different Filenames (Optional)

If you prefer to use different filenames, simply update the image sources in `index.html`:

1. Open `index.html` in a text editor
2. Search for the image filename you want to change (e.g., `family-1.jpg`)
3. Replace it with your new filename
4. Save the file

Example:
```html
<!-- Before -->
<img src="images/family-1.jpg" alt="Family portrait session">

<!-- After (if you named your file differently) -->
<img src="images/my-custom-name.jpg" alt="Family portrait session">
```

## Adding More Images

To add more portfolio images:

1. **Add the image file** to the `images/` folder
2. **Update index.html** by copying an existing portfolio item and modifying it:

```html
<div class="portfolio-item">
    <img src="images/your-new-image.jpg" alt="Descriptive alt text">
</div>
```

## Current Placeholder Setup

The website currently uses Unsplash placeholder images via URL. To download these placeholders:

1. Open the website in a browser
2. Right-click on each image → "Save Image As..."
3. Save with the appropriate filename from the list above
4. Edit/replace with your actual photos when ready

## Pro Tips

✨ **Consistency**: Keep similar lighting and editing style across portfolio images
📐 **Aspect Ratio**: Maintain the 4:5 ratio for portfolio images for a clean grid
🎨 **Alt Text**: Update the `alt` attributes in HTML to describe your actual photos
⚡ **Performance**: Always optimize images before uploading to keep your site fast
📱 **Mobile**: Test your images on mobile devices to ensure they look great everywhere

## Need Help?

If you need to make more advanced customizations, the main files to edit are:
- `index.html` - Structure and content
- `styles.css` - Visual styling
- `script.js` - Interactive features

---

**Questions?** Feel free to reach out for assistance!

