# diegoacanales.github.io

Personal academic website for Diego A. Canales.

**Live site:** https://diegoacanales.github.io

## Quick Start

### Option 1: GitHub Pages (Recommended)

1. Create a new repository named `diegoacanales.github.io` on GitHub
2. Push this folder to the repository
3. Go to Settings → Pages → Enable GitHub Pages from `main` branch
4. Site will be live at `https://diegoacanales.github.io`

### Option 2: Local Development

```bash
# Install Jekyll (requires Ruby)
gem install bundler jekyll

# Install dependencies
bundle install

# Run local server
bundle exec jekyll serve

# Open http://localhost:4000
```

## File Structure

```
diegoacanales.github.io/
├── _config.yml          # Site configuration
├── _layouts/
│   └── default.html     # Main HTML template
├── _pages/
│   ├── research.md      # Research & publications
│   ├── teaching.md      # Teaching information
│   └── cv.md            # Curriculum vitae
├── assets/
│   ├── css/
│   │   └── main.css     # Stylesheet
│   ├── img/             # Images (add profile.jpg here)
│   └── pdf/             # PDFs (papers, CV)
├── index.md             # Home/About page
├── Gemfile              # Ruby dependencies
└── README.md            # This file
```

## Customization Checklist

- [ ] Add `assets/img/profile.jpg` (your photo)
- [ ] Update `_config.yml` with your details
- [ ] Edit `index.md` with your bio
- [ ] Add papers to `_pages/research.md`
- [ ] Upload PDFs to `assets/pdf/`
- [ ] Update `_pages/teaching.md` with your courses
- [ ] Upload CV as `assets/pdf/canales_cv.pdf`
- [ ] (Optional) Add Google Analytics ID to `_config.yml`

## Adding a New Paper

1. Upload PDF to `assets/pdf/`
2. Add entry to `_pages/research.md`:

```markdown
<div class="publication">
  <h3>Paper Title</h3>
  <p class="authors">Your Name, Coauthor Name</p>
  <p class="venue"><em>Journal Name</em>, Year</p>
  <p class="abstract">
    Abstract text here...
  </p>
  <p class="links">
    <a href="{{ '/assets/pdf/filename.pdf' | relative_url }}" class="btn">PDF</a>
    <a href="https://doi.org/XXXXX" class="btn">DOI</a>
    <a href="https://github.com/username/repo" class="btn">Code</a>
  </p>
</div>
```

## LaTeX Support

Math is enabled via MathJax. Use standard LaTeX syntax:

- Inline: `$E[Y|X] = \alpha + \beta X$`
- Display: `$$\sum_{i=1}^{n} x_i$$`

## Connecting to Your Research Repos

When you publish a paper, make the GitHub repo public and link it:

```markdown
<a href="https://github.com/diegoacanales/momentum-primaries" class="btn">Code</a>
```

## Custom Domain (Optional)

To use a custom domain like `diegocanales.com`:

1. Buy domain from Namecheap, Google Domains, etc.
2. Add `CNAME` file with your domain
3. Configure DNS with your registrar
4. Enable HTTPS in GitHub Pages settings

## License

Content © Diego A. Canales. Code is MIT licensed.
