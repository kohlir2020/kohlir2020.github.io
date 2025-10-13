# Personal Website - Raunit Kohli

A minimal Jekyll site built with the Cayman theme for GitHub Pages, showcasing projects, publications, and research work.

## Development Setup

### Prerequisites
- Ruby (2.7 or higher)
- Bundler gem

### Running Locally

1. Install dependencies:
   ```bash
   bundle install
   ```

2. Serve the site locally:
   ```bash
   bundle exec jekyll serve
   ```

3. Open your browser to `http://localhost:4000`

The site will automatically rebuild when you make changes to files.

## Site Structure

```
├── _config.yml          # Site configuration
├── _layouts/
│   └── default.html     # Main layout template
├── _includes/
│   ├── nav.html         # Navigation component
│   └── footer.html      # Footer component
├── _projects/           # Project collection
├── _publications/       # Publications collection
├── assets/
│   ├── css/
│   │   └── site.css     # Custom styles
│   └── img/             # Images
└── content/             # Static content (PDFs, etc.)
```

## Adding Content

### Adding a Project

Create a new file in `_projects/` directory:

```markdown
---
title: "Project Title"
description: "Brief description of the project"
date: 2024-01-15
tags: [tag1, tag2]
---

## Project Description

Your project content here...
```

### Adding a Publication

Create a new file in `_publications/` directory:

```markdown
---
title: "Publication Title"
authors: "Author 1, Author 2"
venue: "Conference/Journal Name"
date: 2024-01-15
pdf_url: "/path/to/paper.pdf"
---

## Abstract

Your publication abstract here...
```

## Navigation

The navigation is responsive and includes:
- **Home**: Main landing page (`/`)
- **Projects**: Collection of projects (`/projects/`)
- **Publications**: Academic publications (`/publications/`)
- **About**: About page (`/about/`)
- **CV**: Direct link to resume PDF
- **Contact**: Contact information (`/contact/`)

### Navigation Features
- Fully accessible with ARIA labels and keyboard navigation
- Active page highlighting
- Mobile-responsive hamburger menu
- Focus management for screen readers

## Customization

### Theme Colors
The site uses the Cayman theme with custom CSS. Main colors can be modified in `assets/css/site.css`:
- Primary green: `#159957`
- Secondary blue: `#155799`
- Link color: `#1e6bb8`

### Social Links
Update the social links in `_includes/footer.html` with your actual URLs.

### Site Configuration
Edit `_config.yml` to update:
- Site title and description
- URL and social media links
- SEO settings

## Deployment

The site automatically deploys to GitHub Pages when you push to the `main` branch. Make sure GitHub Pages is enabled in your repository settings and set to deploy from the `main` branch.

## Accessibility Features

- Semantic HTML structure
- ARIA labels and roles
- Keyboard navigation support
- Focus indicators
- Screen reader friendly
- Color contrast compliance

## License

This project is open source. Feel free to use it as a template for your own site.