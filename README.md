# VoidRunner.dev

Official website for VoidRunner - AI-Powered Serverless Development Platform.

## Quick Start

```bash
# Clone the repository
git clone https://github.com/voidrunnerhq/voidrunner.dev.git
cd voidrunner.dev

# Install Hugo (if not already installed)
# macOS
brew install hugo

# Ubuntu/Debian
sudo apt install hugo

# Windows (using Chocolatey)
choco install hugo

# Add the theme as a submodule
git submodule add https://github.com/chaoming/hugo-saasify-theme.git themes/hugo-saasify-theme

# Update submodules
git submodule update --init --recursive

# Install npm dependencies (for PostCSS)
npm install

# Start development server
hugo server -D

# Build for production
hugo --minify --gc --cleanDestinationDir
```

## Project Structure

```
voidrunner.dev/
├── config.yaml              # Hugo configuration
├── content/                  # Site content (Markdown)
│   ├── _index.md            # Homepage
│   ├── features/            # Features pages
│   ├── pricing/             # Pricing page
│   ├── docs/                # Documentation
│   └── blog/                # Blog posts
├── static/                  # Static assets
│   ├── images/              # Images and logos
│   ├── _headers             # Cloudflare security headers
│   └── _redirects           # URL redirects
├── layouts/                 # Custom Hugo templates
└── themes/                  # Hugo themes
```

## Development

### Local Development

1. **Start the development server:**

   ```bash
   hugo server -D --bind 0.0.0.0 --baseURL http://localhost:1313
   ```

2. **Access the site:**
   - Local: http://localhost:1313
   - Network: http://your-ip:1313

### Content Management

- **Homepage:** Edit `content/_index.md`
- **Features:** Edit `content/features/_index.md`
- **Pricing:** Edit `content/pricing/_index.md`
- **Blog posts:** Add new `.md` files to `content/blog/`

### Adding Images

1. Place images in `static/images/`
2. Reference them in Markdown: `![Alt text](/images/filename.png)`
3. Optimize images before adding (WebP format preferred)

### Customization

- **Styling:** Edit `assets/css/custom.css`
- **JavaScript:** Edit `assets/js/custom.js`
- **Templates:** Add custom layouts in `layouts/`

## Deployment

### Automatic Deployment (Recommended)

The site automatically deploys to Cloudflare Pages when you push to the `main` branch via GitHub Actions.

**Required Secrets:**

- `CLOUDFLARE_API_TOKEN`: Cloudflare API token with Pages permissions
- `CLOUDFLARE_ACCOUNT_ID`: Your Cloudflare account ID

### Manual Deployment

1. **Build the site:**

   ```bash
   hugo --minify --gc --cleanDestinationDir
   ```

2. **Deploy to Cloudflare Pages:**
   - Upload the `public/` directory
   - Or use Wrangler CLI:
     ```bash
     npx wrangler pages deploy public
     ```

## Configuration

### Environment Variables

Set these in your deployment environment:

- `HUGO_ENV=production` (for production builds)
- `HUGO_VERSION=latest` (Hugo version for Cloudflare Pages)

### Site Configuration

Key configuration options in `config.yaml`:

```yaml
baseURL: "https://voidrunner.dev"
title: "VoidRunner - AI-Powered Serverless Development Platform"

params:
  author: "VoidRunner Team"
  description: "Deploy AI applications in minutes, not hours..."

  # Analytics
  google_analytics: "G-XXXXXXXXXX"

  # Social media
  social:
    github: "https://github.com/voidrunnerhq"
    twitter: "https://twitter.com/voidrunnerhq"
```

## Performance Optimization

### Built-in Optimizations

- **Minification:** HTML, CSS, and JS are automatically minified
- **Image Processing:** Hugo's built-in image processing
- **Cloudflare CDN:** Global content delivery and caching
- **Security Headers:** Comprehensive security headers via `_headers`

### Performance Best Practices

1. **Optimize images:**

   ```bash
   # Convert to WebP
   cwebp -q 85 input.png -o output.webp

   # Resize large images
   magick input.jpg -resize 1200x630 output.jpg
   ```

2. **Minimize external dependencies**
3. **Use Hugo's resource bundling for CSS/JS**

## SEO Optimization

### Built-in SEO Features

- **Structured Data:** JSON-LD markup for rich snippets
- **Meta Tags:** Open Graph and Twitter Card support
- **Sitemap:** Automatically generated
- **Robots.txt:** Search engine directives

### SEO Checklist

- [ ] Unique page titles and descriptions
- [ ] Optimized images with alt text
- [ ] Internal linking structure
- [ ] Fast loading times (<3 seconds)
- [ ] Mobile-responsive design
- [ ] HTTPS enabled

## Monitoring and Analytics

### Analytics Setup

1. **Google Analytics:**

   ```yaml
   params:
     google_analytics: "G-XXXXXXXXXX"
   ```

2. **Cloudflare Analytics:**
   - Available in Cloudflare dashboard
   - Real User Monitoring (RUM)
   - Core Web Vitals tracking

### Performance Monitoring

- **Lighthouse:** Run regular audits
- **PageSpeed Insights:** Monitor Core Web Vitals
- **GTmetrix:** Comprehensive performance analysis

## Contributing

1. **Fork the repository**
2. **Create a feature branch:** `git checkout -b feature/amazing-feature`
3. **Make your changes**
4. **Test locally:** `hugo server -D`
5. **Commit your changes:** `git commit -m 'Add amazing feature'`
6. **Push to the branch:** `git push origin feature/amazing-feature`
7. **Open a Pull Request**

### Content Guidelines

- Use clear, concise language
- Follow the established tone and style
- Optimize images before adding
- Test all links and functionality
- Ensure mobile responsiveness

## Support

- **Documentation:** [VoidRunner Docs](https://docs.voidrunner.dev)
- **Issues:** [GitHub Issues](https://github.com/voidrunnerhq/voidrunner.dev/issues)
- **Discord:** [VoidRunner Community](https://discord.gg/voidrunner)
- **Email:** hello@voidrunner.dev

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **Hugo:** Static site generator
- **Hugo Saasify Theme:** Base theme for SaaS websites
- **Cloudflare Pages:** Hosting and CDN
- **GitHub Actions:** CI/CD pipeline
