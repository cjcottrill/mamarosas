# 🍕 Mama Rosa's Pizza

A responsive, mobile-first Progressive Web App (PWA) for a pizza restaurant menu.

## Features

✨ **Progressive Web App (PWA)**
- Install as app on mobile devices
- Works offline with service worker
- Fast loading with caching strategy

📱 **Fully Responsive Design**
- Works perfectly on mobile, tablet, and desktop
- Touch-friendly interface
- Optimized for all screen sizes

🎨 **Modern UI**
- Clean, professional design
- Smooth animations and transitions
- Easy to customize colors and branding

📋 **Menu Management**
- Organized pizza categories
- Pricing for different sizes
- Sides and extras section
- Easy to add/edit items

## Getting Started

1. **Clone the repository** (if needed)
2. **Host the files** on a web server or serve locally
3. **Access via HTTPS** (required for PWA features)
4. **Install the app** on mobile or desktop

## Local Development

To test locally, you can use a simple HTTP server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (with http-server package)
npx http-server

# Using PHP
php -S localhost:8000
```

Then navigate to `http://localhost:8000` in your browser.

**Note:** Service Worker requires HTTPS in production (localhost works in development).

## File Structure

```
mamarosas/
├── index.html          # Main page with menu
├── style.css           # Styling and responsive design
├── manifest.json       # PWA configuration
├── service-worker.js   # Offline functionality
├── .gitignore         # Git ignore rules
├── README.md          # This file
└── images/            # Pizza images and icons
    ├── icon-192.png
    ├── icon-512.png
    └── (other images)
```

## Customization

### Change Colors
Edit the CSS variables in `style.css`:
```css
:root {
    --primary-color: #d32f2f;      /* Red */
    --secondary-color: #f57c00;    /* Orange */
    /* ... other colors */
}
```

### Update Restaurant Info
- Edit the `<title>` and `<meta>` tags in `index.html`
- Update the manifest.json with your restaurant name
- Change the header content in `index.html`

### Add/Edit Menu Items
Open `index.html` and modify the menu items in the `.menu-grid` sections.

## Images Needed

To complete the PWA, you'll need these images in the `images/` folder:
- `icon-192.png` - 192x192 app icon
- `icon-512.png` - 512x512 app icon
- `icon-maskable-192.png` - 192x192 maskable icon
- `icon-maskable-512.png` - 512x512 maskable icon
- `apple-touch-icon.png` - 180x180 Apple touch icon
- `favicon.png` - 32x32 favicon
- `screenshot-540x720.png` - Mobile screenshot
- `screenshot-1280x720.png` - Desktop screenshot

**Placeholder:** Currently using emoji (🍕) for pizza images.

## Deployment

### Netlify
1. Connect your GitHub repo to Netlify
2. Set build command: none (static files)
3. Deploy!

### Vercel
1. Connect your GitHub repo to Vercel
2. Deploy with one click!

### GitHub Pages
1. Push to GitHub
2. Enable GitHub Pages in repo settings
3. Select the `main` branch as source

**Note:** GitHub Pages uses `https://` by default, so PWA features work perfectly.

## Browser Support

| Feature | Chrome | Firefox | Safari | Edge |
|---------|--------|---------|--------|------|
| PWA Install | ✅ | ✅ | ✅ | ✅ |
| Service Worker | ✅ | ✅ | ✅ | ✅ |
| Offline Mode | ✅ | ✅ | ✅ | ✅ |
| Responsive Design | ✅ | ✅ | ✅ | ✅ |

## Performance Tips

- Keep images optimized (use WebP when possible)
- Lazy load images on scroll (add JavaScript if needed)
- Minify CSS/JS for production
- Use a CDN for faster delivery

## License

Free to use and modify for your restaurant.

## Support

For issues or feature requests, create an issue on GitHub.

---

**Made with ❤️ for pizza lovers**
