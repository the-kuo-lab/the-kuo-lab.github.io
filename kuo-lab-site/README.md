# The Kuo Lab Website

Static site built with Jekyll, hosted on GitHub Pages at `the-kuo-lab.github.io`.

## Quick Setup

### 1. Push to GitHub

Upload all files to your `the-kuo-lab/the-kuo-lab.github.io` repository.

### 2. Enable GitHub Pages

Go to: **Repository Settings → Pages → Source → Deploy from branch → main → / (root)**

Your site will be live at `https://the-kuo-lab.github.io` within ~2 minutes.

### 3. Local preview (optional)

```bash
gem install bundler jekyll
bundle install
bundle exec jekyll serve
# Open http://localhost:4000
```

---

## Customizing Content

### Add a publication
Edit `pages/publications.html` — copy a `.pub-item` block and fill in your details.

### Add a team member
Edit `pages/team.html` — copy a `.team-card` block and fill in name, role, bio.
To add a photo: place image in `assets/images/` and replace the `.team-avatar` div with `<img src="/assets/images/yourphoto.jpg" alt="Name" />`.

### Update lab news
Edit `index.html` and update the `.news-list` section.

### Contact form
The contact form uses [Formspree](https://formspree.io) — free tier supports 50 submissions/month.
1. Sign up at formspree.io
2. Create a form
3. Replace `YOUR_FORM_ID` in `pages/contact.html` with your form ID

---

## File Structure

```
├── _layouts/
│   └── default.html       # Main HTML template (nav, footer)
├── assets/
│   ├── css/main.css       # All styles
│   ├── js/main.js         # Mobile nav toggle
│   └── images/            # Add your photos here
├── pages/
│   ├── research.html
│   ├── publications.html
│   ├── team.html
│   ├── join.html
│   └── contact.html
├── index.html             # Home page
├── _config.yml            # Jekyll config
└── Gemfile
```
