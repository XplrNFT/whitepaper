# XPLR Whitepaper - MkDocs Deployment Guide

This is the complete XPLR Whitepaper documentation built with MkDocs and Material theme.

## Quick Start

### Prerequisites
- Python 3.8+
- Git
- GitHub account

### Local Development

1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/xplr-whitepaper.git
cd xplr-whitepaper
```

2. Install dependencies:
```bash
pip install mkdocs mkdocs-material
```

3. Run the development server:
```bash
mkdocs serve
```

The site will be available at `http://localhost:8000`

### Deploy to GitHub Pages

1. Create a new repository on GitHub named `xplr-whitepaper`

2. Add the remote and push:
```bash
git remote add origin https://github.com/YOUR_USERNAME/xplr-whitepaper.git
git branch -M main
git push -u origin main
```

3. GitHub Actions will automatically deploy the site to GitHub Pages

4. Enable GitHub Pages in repository settings:
   - Go to Settings → Pages
   - Select "Deploy from a branch"
   - Choose `gh-pages` branch and `/ (root)` folder
   - Click Save

5. Your site will be available at: `https://YOUR_USERNAME.github.io/xplr-whitepaper/`

## Project Structure

```
xplr-whitepaper/
├── docs/                          # Documentation source files
│   ├── index.md                   # Home page
│   ├── welcome/                   # Welcome section
│   ├── core-concept/              # Core concepts
│   ├── xplr-dao/                  # DAO information
│   ├── faq/                       # FAQ section
│   └── link/                      # External links
├── site/                          # Built site (auto-generated)
├── mkdocs.yml                     # MkDocs configuration
├── .github/workflows/deploy.yml   # GitHub Actions workflow
└── README.md                      # This file
```

## Configuration

Edit `mkdocs.yml` to customize:
- Site name and description
- Theme colors and features
- Navigation structure
- Markdown extensions

## Content Guidelines

- All pages should be in Markdown format (.md)
- Use relative links for internal navigation
- Images should be placed in `docs/assets/` directory
- Follow the existing folder structure for organization

## Building the Site

To build the site locally:
```bash
mkdocs build
```

The built site will be in the `site/` directory.

## Support

For issues or questions, please refer to:
- [MkDocs Documentation](https://www.mkdocs.org/)
- [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)

## License

This documentation is part of the XPLR project.
