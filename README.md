# Mithl-OS Website

> **Official project website for Mithl-OS - The Modern OS for Creators**

This directory contains the static website files for the Mithl-OS project, showcasing the operating system's features, vision, and contribution guidelines.

---

## 📁 File Structure

```
web/
├── index.html              # Homepage - Main landing page
├── features.html           # Features page - Detailed feature showcase
├── contribute.html         # Contribution page - Guidelines for contributors
├── style.css              # Main stylesheet - Unified design system
├── googlee42c15053e106686.html  # Google Search Console verification
└── README.md              # This file
```

---

## 🎨 Design System

The website uses the **Glass Prism** design language, featuring:

- **Modern Glassmorphism**: Transparent, frosted glass effects with subtle blur
- **Vibrant Color Palette**: 
  - Primary: `#00d4ff` (Cyan)
  - Accent: `#ffeb3b` (Yellow)
  - Background: Dark gradient (`#0a0e27` to `#1a1f3a`)
- **Typography**: Inter font family (Google Fonts)
- **Responsive Design**: Mobile-friendly layouts with smooth transitions
- **Micro-animations**: Hover effects and interactive elements

---

## 🚀 Pages Overview

### 1. **index.html** - Homepage
The main landing page featuring:
- Hero section with tagline: "Fast. Beautiful. Yours."
- Three key value propositions:
  - ⚡ Direct-to-Metal performance
  - 🎨 Glass Prism UI
  - 🛡️ Rock Solid stability
- Latest updates section showcasing v0.5 release and upcoming features

### 2. **features.html** - Features Page
Detailed showcase of Mithl-OS capabilities:
- Performance features (instant boot, direct hardware access)
- Developer tools (GCC/Make support, POSIX compatibility)
- Visual design (Glass Prism UI, distraction-free workspace)
- Future roadmap (Project Curiosity, advanced window tiling)

### 3. **contribute.html** - Contribution Guidelines
Information for potential contributors:
- How to get started
- Contribution areas (kernel development, UI/UX, documentation)
- Community guidelines
- Links to GitHub repository

---

## 🛠️ Local Development

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- Optional: A local web server for testing

### Running Locally

**Option 1: Direct File Access**
Simply open `index.html` in your web browser:
```bash
# From the web directory
open index.html
# or
xdg-open index.html  # Linux
```

**Option 2: Local Web Server (Recommended)**
Using Python's built-in HTTP server:
```bash
# Python 3
python3 -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

Then navigate to `http://localhost:8000` in your browser.

**Option 3: Using Node.js**
```bash
# Install http-server globally
npm install -g http-server

# Run server
http-server -p 8000
```

---

## 🌐 Deployment

The website is designed to be deployed as a static site and is compatible with:

- **GitHub Pages** (currently deployed)
- **Netlify**
- **Vercel**
- **AWS S3 + CloudFront**
- Any static hosting service

### GitHub Pages Deployment
The site is automatically deployed from the repository. To update:
1. Make changes to the HTML/CSS files
2. Commit and push to the main branch
3. GitHub Pages will automatically rebuild and deploy

---

## 🎯 Key Features

### Responsive Design
- Mobile-first approach
- Breakpoints for tablets and desktops
- Touch-friendly navigation

### SEO Optimized
- Semantic HTML5 structure
- Meta tags for social sharing
- Descriptive titles and headings
- Google Search Console verification

### Performance
- Minimal dependencies (only Google Fonts)
- Optimized CSS with CSS variables
- Fast loading times
- No JavaScript framework overhead

### Accessibility
- Proper heading hierarchy
- ARIA labels where needed
- High contrast ratios
- Keyboard navigation support

---

## 🎨 Customization

### Color Scheme
Colors are defined as CSS variables in `style.css`:
```css
:root {
    --primary: #00d4ff;
    --accent: #ffeb3b;
    --bg-dark: #0a0e27;
    --bg-darker: #1a1f3a;
    --glass-bg: rgba(255, 255, 255, 0.05);
    --glass-border: rgba(255, 255, 255, 0.1);
}
```

### Typography
The site uses the Inter font family. To change:
1. Update the Google Fonts link in the `<head>` section
2. Modify the `font-family` in CSS

### Layout
The grid system uses CSS Grid and Flexbox for responsive layouts. Adjust breakpoints in the media queries section of `style.css`.

---

## 📝 Content Updates

### Adding New Features
1. Edit `features.html`
2. Add a new card in the appropriate section
3. Follow the existing HTML structure for consistency

### Updating Latest News
1. Edit `index.html`
2. Modify the "Latest Updates" section
3. Use the existing badge styles for version tags

### Modifying Navigation
Update the navigation in all three HTML files to maintain consistency:
```html
<nav>
    <div class="logo">Mithl-OS</div>
    <div class="nav-links">
        <a href="index.html">Home</a>
        <a href="features.html">Features</a>
        <a href="contribute.html">Contribute</a>
        <a href="https://github.com/DoguparthiAakash/Mithl-OS" target="_blank">GitHub</a>
    </div>
</nav>
```

---

## 🔗 External Links

- **GitHub Repository**: https://github.com/DoguparthiAakash/Mithl-OS
- **Live Website**: https://doguparthiaakash.github.io/Mithl-OS/ (or your custom domain)

---

## 🤝 Contributing to the Website

We welcome contributions to improve the website! Here's how:

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/improve-website
   ```
3. **Make your changes**
   - Ensure responsive design is maintained
   - Test on multiple browsers
   - Follow the existing design language
4. **Commit your changes**
   ```bash
   git commit -m "Improve website accessibility"
   ```
5. **Push and create a Pull Request**

### Website Contribution Guidelines
- Maintain the Glass Prism design aesthetic
- Ensure mobile responsiveness
- Test on Chrome, Firefox, and Safari
- Optimize images and assets
- Follow semantic HTML practices
- Keep CSS organized and commented

---

## 📄 License

The website content and design are part of the Mithl-OS project. Please refer to the main project LICENSE file for details.

---

## 📞 Contact

For questions or suggestions about the website:
- Open an issue on GitHub
- Submit a pull request
- Contact the maintainers through the repository

---

*Built with ❤️ for the Mithl-OS community*
