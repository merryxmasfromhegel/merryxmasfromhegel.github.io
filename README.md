# manishoza.ca — Jekyll Site

A simple Jekyll site for Manish Oza's academic portfolio.

## Getting Started

### Prerequisites
- Ruby 3.x
- Bundler (`gem install bundler`)

### Local Development

```bash
# Install dependencies
bundle install

# Serve locally with live reload
bundle exec jekyll serve --livereload
```

Visit `http://localhost:4000` in your browser.

### Building for Production

```bash
bundle exec jekyll build
```

Output will be in the `_site/` folder.

---

## Deployment: GitHub Pages (Free Hosting)

1. Create a GitHub repository named `manishoza.ca` (or any name).
2. Push this folder to the repo.
3. Go to **Settings → Pages** in the repo.
4. Under **Source**, select `Deploy from a branch` → `main` → `/ (root)`.
5. GitHub will build and deploy your site automatically.

If using a custom domain (manishoza.ca):
- Add a file named `CNAME` to this folder containing just: `manishoza.ca`
- Point your domain's DNS to GitHub Pages (see GitHub docs).

---

## Adding Content

### Research & Teaching pages
Edit `_pages/research.md` and `_pages/teaching.md` — they use standard Markdown.

### PDF files
Place any PDF files (CV, papers, etc.) in `assets/pdf/` and link to them like:
```markdown
[My Paper]({{ '/assets/pdf/paper.pdf' | relative_url }})
```

### Updating the layout or style
- Layout: `_layouts/default.html`
- Styles: `assets/css/style.css`
