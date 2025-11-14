# GitHub Pages Root Site with Jekyll

A simple, colorful Jekyll theme for the GitHub Pages root site at https://robinali34.github.io/

## Features

- 🎨 Simple, colorful design with gradient backgrounds
- 📱 Fully responsive layout
- 🚀 Automatic deployment via GitHub Actions
- 🎯 Color-coded blog links
- ⚡ Fast and lightweight

## Setup

1. **Create the repository on GitHub:**
   - Repository name: `robinali34.github.io` (must match your username exactly)
   - Make it public

2. **Push this code to the repository:**
   ```bash
   git remote add origin https://github.com/robinali34/robinali34.github.io.git
   git branch -M main
   git push -u origin main
   ```

3. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Under "Source", select "GitHub Actions"
   - The workflow will automatically build and deploy your Jekyll site

4. **Access your site:**
   - After deployment, your site will be available at: https://robinali34.github.io/

## Local Development

To run Jekyll locally:

```bash
# Install dependencies
bundle install

# Serve the site locally
bundle exec jekyll serve

# Visit http://localhost:4000
```

## Customization

### Colors

Edit `_config.yml` to customize colors:

```yaml
theme_colors:
  primary: "#667eea"
  secondary: "#764ba2"
  accent: "#f093fb"
```

### Blog Links

Add or modify blog links in `_config.yml`:

```yaml
blogs:
  - name: "Blog Name"
    url: "https://example.com"
    description: "Blog description"
    color: "#hexcolor"
```

### Styling

Modify `assets/css/main.css` to customize the theme appearance.

## Structure

```
.
├── _config.yml          # Jekyll configuration
├── _layouts/
│   └── default.html     # Default layout template
├── assets/
│   └── css/
│       └── main.css     # Main stylesheet
├── index.html           # Homepage
├── Gemfile              # Ruby dependencies
└── .github/
    └── workflows/
        └── deploy.yml   # GitHub Actions workflow
```

## License

MIT

