# Deployment Guide

## Overview
Your Jekyll site is fully configured and ready for deployment to GitHub Pages. The site includes comprehensive SEO optimization, accessibility compliance (WCAG AA), and mobile-first responsive design.

## Deployment to GitHub Pages

### 1. Push to GitHub Repository
```bash
# Add all files
git add .

# Commit changes
git commit -m "Complete Jekyll site with accessibility enhancements"

# Push to GitHub
git push origin main
```

### 2. Enable GitHub Pages
1. Go to your repository settings on GitHub
2. Navigate to "Pages" in the left sidebar
3. Under "Source", select "Deploy from a branch"
4. Choose "main" branch and "/ (root)" folder
5. Click "Save"

GitHub Pages will automatically build your Jekyll site (no local build required).

## Site Features

### ✅ SEO Optimization
- Complete meta tags and Open Graph data
- XML sitemap generation
- RSS feed
- Structured data (JSON-LD) for Person, Projects, and Publications
- robots.txt configuration
- Favicon implementation

### ✅ Accessibility (WCAG AA Compliant)
- Semantic HTML5 structure
- Proper ARIA labels and roles
- Focus management and keyboard navigation
- High contrast support
- Screen reader compatibility
- 44px minimum touch targets for mobile
- Skip-to-content links
- Reduced motion support

### ✅ Mobile-First Design
- Responsive layout across all devices
- Touch-friendly navigation
- Optimized typography scaling
- Enhanced mobile menu with focus trapping
- Swipe indicators and gestures

### ✅ Performance Features
- Minimal CSS and JavaScript
- Optimized images and assets
- Efficient caching headers
- Clean, semantic markup

## Site Structure

```
/
├── _config.yml           # Jekyll configuration with SEO settings
├── _layouts/
│   └── default.html     # Enhanced layout with structured data
├── _includes/
│   ├── nav.html         # Accessible navigation with focus management
│   ├── head-seo.html    # SEO meta tags and structured data
│   └── structured-data/ # JSON-LD schema markup
├── _pages/              # Site pages
├── _projects/           # Project collection
├── _publications/       # Publication collection
├── assets/
│   ├── css/
│   │   └── site.css     # Comprehensive styling with accessibility
│   └── images/          # Favicon and site images
├── robots.txt           # Search engine directives
└── content/             # Original content files
```

## Local Development (Optional)

If you want to test locally before deploying:

### Install Development Tools (macOS)
```bash
# Install Xcode command line tools
xcode-select --install

# Install Homebrew (if not already installed)
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install rbenv and ruby-build
brew install rbenv ruby-build

# Install and use Ruby 3.x
rbenv install 3.2.0
rbenv global 3.2.0

# Add to your shell profile (~/.zshrc)
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(rbenv init -)"' >> ~/.zshrc
source ~/.zshrc
```

### Local Jekyll Setup
```bash
# Install bundler
gem install bundler

# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve --livereload

# Site will be available at http://localhost:4000
```

## Validation Tools

### Test Accessibility
- [WAVE Web Accessibility Evaluator](https://wave.webaim.org/)
- [axe DevTools browser extension](https://www.deque.com/axe/devtools/)

### Test SEO
- [Google Search Console](https://search.google.com/search-console)
- [Google Rich Results Test](https://search.google.com/test/rich-results)

### Test Performance
- [Google PageSpeed Insights](https://pagespeed.web.dev/)
- [GTmetrix](https://gtmetrix.com/)

### Test Mobile Usability
- [Google Mobile-Friendly Test](https://search.google.com/test/mobile-friendly)

## Customization

### Colors
The site uses the Cayman theme color scheme. To customize:
- Primary: #159957 (green gradient start)
- Secondary: #155799 (blue gradient end)  
- Accent: #ffbf47 (focus/highlight yellow)
- Text: White on dark backgrounds

### Typography
- Headers: System fonts with fallbacks
- Body: Optimized for readability across devices
- Responsive scaling for mobile devices

### Navigation
The navigation is fully accessible with:
- Keyboard navigation support
- Focus trapping in mobile menu
- ESC key to close mobile menu
- ARIA labels and roles

## Troubleshooting

### Common Issues
1. **Site not updating**: GitHub Pages can take 10-15 minutes to deploy changes
2. **Custom domain**: Configure in repository settings → Pages → Custom domain
3. **404 errors**: Check that your repository is named correctly for GitHub Pages

### Support Resources
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Jekyll Theme Cayman](https://github.com/pages-themes/cayman)

## Next Steps

1. **Deploy to GitHub Pages** following the steps above
2. **Test all functionality** using the validation tools
3. **Monitor performance** with Google Search Console
4. **Consider custom domain** for professional branding
5. **Regular content updates** to maintain SEO ranking

Your site is professionally configured and ready for deployment! 🚀