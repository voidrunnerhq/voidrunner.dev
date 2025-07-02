# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the VoidRunner.dev website - a Hugo-based static site for the VoidRunner AI-Powered Serverless Development Platform. The site uses the `hugo-saasify-theme` as a git submodule and is deployed to Cloudflare Pages.

## Development Commands

### Local Development
```bash
# Start development server with drafts enabled
npm run dev
# Alternative: hugo server -D --disableFastRender

# Start development server accessible from network
hugo server -D --bind 0.0.0.0 --baseURL http://localhost:1313
```

### Building
```bash
# Production build
npm run build
# Alternative: hugo --minify --gc --cleanDestinationDir

# Preview build (with relative URLs)
npm run build:preview

# Clean build artifacts
npm run clean
```

### Dependencies
```bash
# Install npm dependencies (PostCSS, Tailwind CSS)
npm install

# Update git submodules (theme)
git submodule update --init --recursive

# Security audit
npm run security-audit

# Update dependencies
npm run update-deps
```

## Architecture & Structure

### Hugo Configuration
- **Main config**: `config.yaml` contains all site configuration, including theme settings, menu structure, and deployment parameters
- **Theme**: Uses `hugo-saasify-theme` as a git submodule in `themes/` directory
- **Content structure**: Organized with content types for blog, features, pricing, and docs

### Content Management
- **Homepage**: `content/_index.md`
- **Features**: `content/features/_index.md` and individual feature pages
- **Pricing**: `content/pricing/_index.md`
- **Blog**: Individual `.md` files in `content/blog/`
- **Docs**: Documentation pages in `content/docs/`

### Asset Management
- **Static assets**: Place in `static/` directory (copied as-is to `public/`)
- **Images**: Organized in `static/images/` with subdirectories for blog, company, logos, social
- **Headers/Redirects**: Cloudflare-specific files in `static/_headers` and `static/_redirects`

### Styling System
- **Framework**: TailwindCSS configured via `themes/hugo-saasify-theme/tailwind.config.js`
- **Custom colors**: Primary (blue tones) and secondary (purple tones) color palettes
- **Typography**: Inter for body text, Plus Jakarta Sans for headings
- **PostCSS**: Configured for Tailwind processing and autoprefixer

## Deployment

### Automatic Deployment
- **Trigger**: Push to `main` branch
- **Platform**: Cloudflare Pages via GitHub Actions
- **Workflow**: `.github/workflows/deploy.yml`
- **Build command**: `hugo --minify --gc --cleanDestinationDir`
- **Hugo version**: 0.134.3 (extended)
- **Node version**: 22

### Manual Deployment
```bash
# Using Wrangler CLI
npx wrangler pages deploy public
```

### Environment Configuration
- **Production**: `HUGO_ENV=production`, `HUGO_BASEURL=https://voidrunner.dev`
- **Preview**: `HUGO_ENV=development`, `HUGO_BASEURL=/`
- **Required secrets**: `CLOUDFLARE_API_TOKEN`, `CLOUDFLARE_ACCOUNT_ID`

## Key Integration Points

### Theme Customization
- Theme is a git submodule - avoid editing theme files directly
- Use `layouts/` directory for template overrides
- Custom partials go in `layouts/partials/`
- SEO configuration in `layouts/partials/seo.html`

### Content Types
- **Blog posts**: Support tags, categories, authors taxonomy
- **Features**: Individual feature pages with custom layout
- **Permalinks**: Custom URL structure for blog (`/blog/:year/:month/:day/:slug/`) and features (`/features/:slug/`)

### Performance & SEO
- **Minification**: Enabled for HTML, CSS, JS, JSON, SVG, XML
- **Image processing**: Lanczos resampling, 85% quality
- **Security headers**: Configured via `static/_headers` for Cloudflare
- **Analytics**: Google Analytics and GTM support configured
- **Robots.txt**: Auto-generated with custom rules

## Development Workflow

### Making Changes
1. **Content updates**: Edit markdown files in `content/`
2. **Template changes**: Add overrides in `layouts/` (don't modify theme directly)
3. **Styling**: Work with TailwindCSS classes, theme provides base configuration
4. **Assets**: Add to `static/` directory, optimize images to WebP when possible

### Testing
- Always test locally with `hugo server -D` before deploying
- Check both desktop and mobile responsiveness
- Verify all links and images load correctly
- Test build process with `npm run build` before pushing

### Git Submodule Management
- Theme updates: `git submodule update --remote themes/hugo-saasify-theme`
- When cloning: Always use `git submodule update --init --recursive`
- Submodule is tracked at specific commit - update deliberately

## Performance Considerations
- **Image optimization**: Convert to WebP, resize appropriately
- **Build optimization**: Hugo's resource bundling and minification enabled
- **CDN**: Cloudflare handles global distribution and caching
- **Core Web Vitals**: Monitor via Lighthouse and PageSpeed Insights