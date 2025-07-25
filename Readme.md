# Thomas Carstens - Research Portfolio 🚁

> **Live Site:** https://thomascarstens.github.io/

A thesis-focused portfolio website showcasing robotics research on "Intelligent Systems for Next Generation Drone Functionality" with direct navigation to specific sections of the thesis PDF.

## 🎯 Overview

This portfolio is designed to prominently feature Thomas Carstens' Masters thesis research on lab-to-field robotics using human-drone interaction and crossreality. The site provides:

- **Thesis Navigation**: Direct links to specific sections of the thesis PDF
- **Research Focus**: Detailed overview of the research domain
- **Clean Design**: Minimalist, professional layout focused on the academic work
- **Responsive**: Mobile-friendly design using Bootstrap

## 📁 Project Structure

```
online_portfolio/
├── index.html              # Main homepage (thesis-focused)
├── assets/
│   ├── css/
│   │   └── style.css       # Custom styles + thesis navigation styling
│   ├── img/
│   │   └── profile.png     # Profile image
│   ├── pdfs/
│   │   └── Proceeding-2021-AL-1.2-pages-128-211.pdf  # Thesis PDF
│   ├── js/
│   │   └── main.js         # Main JavaScript functionality
│   └── vendor/             # Bootstrap, jQuery, and other dependencies
├── projects/               # Individual project pages (legacy)
├── node_modules/           # Dependencies for local development
├── package-lock.json       # Dependency lock file
└── README.md              # This file
```

## 🚀 Quick Start

### Local Development

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ThomasCarstens/thomascarstens.github.io.git
   cd thomascarstens.github.io
   ```

2. **Start a local server:**
   ```bash
   # Option 1: Using Python (recommended)
   python -m http.server 8000

   # Option 2: Using Node.js http-server (if installed)
   npx http-server -p 8000

   # Option 3: Using PHP (if available)
   php -S localhost:8000
   ```

3. **Open in browser:**
   Navigate to `http://localhost:8000`

### GitHub Pages Deployment

This site is automatically deployed via GitHub Pages:

1. **Push changes to the `master` branch**
2. **GitHub Pages automatically builds and deploys**
3. **Site is live at:** https://thomascarstens.github.io/

## 📖 Thesis Navigation

The homepage features direct navigation to thesis sections:

- **Introduction** (Page 5): Problem statement and research domains
- **Testbed Environment** (Page 12): UAV spatial localization and system architecture
- **Human-Drone Interfaces** (Page 35): Gesture control and mixed reality interfaces
- **Industrial Deployment** (Page 58): Real-world applications and field testing
- **Conclusion** (Page 81): Research outcomes and future work
- **Problem Statement** (Page 7): Detailed problem definition

### Updating Thesis Sections

To modify the thesis navigation buttons, edit the links in `index.html`:

```html
<a href="assets/pdfs/Proceeding-2021-AL-1.2-pages-128-211.pdf#page=5" target="_blank" class="btn btn-thesis">
  <i class="bx bx-file-blank"></i> Introduction
</a>
```

**Note:** Page numbers are calculated as: `PDF_page_number - 124` (since the thesis starts on page 129 in the proceedings document).

## 🎨 Customization

### Updating Thesis Content

1. **Replace the PDF:**
   - Add your new thesis PDF to `assets/pdfs/`
   - Update the file path in all navigation links in `index.html`

2. **Update Section Links:**
   - Modify the href attributes in the thesis navigation buttons
   - Update section titles and descriptions as needed

3. **Modify Styling:**
   - Edit `assets/css/style.css` to customize colors, fonts, and layout
   - Thesis-specific styles are in the "Thesis Section Styles" section

### Key CSS Classes

- `.thesis`: Main thesis section container
- `.thesis-content`: Content wrapper with background styling
- `.btn-thesis`: Navigation buttons for thesis sections
- `.thesis-navigation`: Container for all navigation elements

## 🛠️ Technical Details

### Dependencies

- **Bootstrap 4**: Responsive grid system and components
- **jQuery**: DOM manipulation and animations
- **Boxicons**: Icon library for navigation buttons
- **Google Fonts**: Typography (Open Sans, Raleway, Poppins)

### Browser Support

- Chrome/Edge: ✅ Full support
- Firefox: ✅ Full support
- Safari: ✅ Full support
- Mobile browsers: ✅ Responsive design

### Performance

- **Lightweight**: Minimal JavaScript, optimized CSS
- **Fast Loading**: Compressed assets, efficient structure
- **SEO Optimized**: Proper meta tags and semantic HTML

## 📝 Content Management

### Adding New Sections

To add new sections to the homepage:

1. **Add HTML section:**
   ```html
   <section id="new-section" class="new-section">
     <div class="container">
       <!-- Your content here -->
     </div>
   </section>
   ```

2. **Add navigation link:**
   ```html
   <li><a href="#new-section"> <span>New Section</span></a></li>
   ```

3. **Add CSS styling:**
   ```css
   .new-section {
     padding: 80px 0;
     /* Your styles here */
   }
   ```

### Updating Profile Information

- **Profile Image**: Replace `assets/img/profile.png`
- **About Text**: Edit the content in the `#about` section
- **Social Links**: Update LinkedIn and GitHub URLs in navigation and about section

## 🚀 Deployment Options

### GitHub Pages (Current)
- **Automatic**: Pushes to `master` branch auto-deploy
- **Custom Domain**: Can be configured in repository settings
- **HTTPS**: Automatically enabled

### Alternative Hosting
- **Netlify**: Drag and drop deployment
- **Vercel**: Git-based deployment
- **Traditional Web Hosting**: Upload files via FTP

## 🔧 Troubleshooting

### Common Issues

1. **PDF Links Not Working:**
   - Ensure PDF file exists in `assets/pdfs/`
   - Check file path spelling in HTML links
   - Verify page numbers are correct

2. **Styling Issues:**
   - Clear browser cache
   - Check CSS file paths
   - Verify Bootstrap dependencies are loading

3. **Local Server Issues:**
   - Try different port: `python -m http.server 3000`
   - Check firewall settings
   - Ensure Python/Node.js is installed

### Development Tips

- **Live Reload**: Use VS Code Live Server extension for automatic refresh
- **CSS Changes**: Hard refresh (Ctrl+F5) to see CSS updates
- **Mobile Testing**: Use browser dev tools device simulation

## 📞 Support

For questions about this portfolio setup:
- **GitHub Issues**: Create an issue in the repository
- **LinkedIn**: [Thomas Carstens](https://www.linkedin.com/in/thomas-carstens-31632468/)
- **Email**: Available through LinkedIn profile

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Last Updated:** January 2025
**Version:** 2.0 (Thesis-focused redesign)
