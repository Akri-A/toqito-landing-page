# Toquito Landing Page

Official landing page for the [toqito](https://github.com/vprusso/toqito) project - an open-source Python library for quantum information theory.

## Overview

This is a Hugo-based static site using the PaperMod theme, designed for deployment on GitHub Pages.

## Prerequisites

- Hugo Extended v0.139.3 or higher
- Git

## Local Development

1. Clone the repository with submodules:
   ```bash
   git clone --recurse-submodules <repository-url>
   cd Toquito_landing_page
   ```

2. Run the development server:
   ```bash
   hugo server -D
   ```

3. Visit http://localhost:1313 to see your site

## Building

To build the site for production:

```bash
hugo --minify
```

The built site will be in the `public/` directory.

## Deployment

This project is configured for automatic deployment to GitHub Pages via GitHub Actions.

- Push to the `main` branch triggers automatic deployment
- Site will be available at your GitHub Pages URL

### Configuring Custom Domain (Optional)

1. Go to repository Settings → Pages
2. Under "Custom domain", enter your domain name
3. Update `baseURL` in `hugo.toml` to match your domain

## Project Structure

```
.
├── archetypes/       # Content templates
├── content/          # Site content
│   ├── blog/        # Blog posts
│   ├── news/        # News updates
│   └── releases/    # Release notes
├── layouts/          # Custom HTML templates
├── static/           # Static assets (images, favicon, etc.)
├── themes/           # Hugo themes (PaperMod)
├── hugo.toml        # Hugo configuration
└── README.md        # This file
```

## Adding Content

### Blog Posts

```bash
hugo new blog/my-post.md
```

### News Updates

```bash
hugo new news/my-update.md
```

### Release Notes

```bash
hugo new releases/v1.0.0.md
```

## License

See [toqito project](https://github.com/vprusso/toqito) for license information.
