# Machine Learning Laboratory Website

This is the official website for the Machine Learning Laboratory at the Department of Engineering and Architecture, University of Trieste.

The lab brings together research from two complementary groups led by:
- **Prof. Sylvio Barbon Junior** (https://barbon.inginf.units.it/)
- **Prof. Andrea De Lorenzo** (https://delorenzo.inginf.units.it/)

## Website: https://meta-group.github.io

### Structure

- `index.html` - Main website
- `styles.css` - Styling
- `images/` - Team photos and other images
- `_config.yml` - GitHub Pages configuration

## How to Update the Website

### Adding Team Members

Edit `index.html` and add new team cards in the appropriate section:

```html
<div class="team-card">
    <img src="images/name.jpg" alt="Name" class="team-photo">
    <h4>Name</h4>
    <p class="role">Position Title</p>
    <p class="bio">Bio or research interests</p>
    <div class="contact-info">
        <p><strong>Email:</strong> <a href="mailto:email@units.it">email@units.it</a></p>
    </div>
</div>
```

### Adding Projects

Edit `index.html` and add new project cards in the Projects section:

```html
<div class="project-card">
    <h3>Project Name</h3>
    <p class="project-meta">Funding: Name | Duration: YYYY-YYYY</p>
    <p>Description...</p>
    <div class="project-details">
        <p><strong>Team:</strong> Names</p>
        <p><strong>Status:</strong> Status</p>
    </div>
</div>
```

### Adding Publications

Edit `index.html` and add new publication items:

```html
<div class="publication-item">
    <h4>Paper Title</h4>
    <p class="authors">Authors</p>
    <p class="venue"><em>Journal/Conference</em>, Year</p>
    <p class="abstract">Abstract...</p>
    <div class="publication-links">
        <a href="#" class="btn-small">PDF</a>
        <a href="#" class="btn-small">DOI</a>
    </div>
</div>
```

### Adding Images

Place image files in the `images/` directory and reference them in HTML as:
```html
<img src="images/filename.jpg" alt="Description">
```

## Local Development

To preview changes locally (if you have a web server):

```bash
# Using Python 3
python -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000
```

Then open `http://localhost:8000` in your browser.

## Deployment

Changes to the `main` branch are automatically deployed to GitHub Pages.

## Customization

### Colors

The website uses CSS variables defined in `styles.css`:

- `--primary-color`: Main color (dark blue)
- `--secondary-color`: Secondary color (blue)
- `--accent-color`: Accent color (orange)

Edit these in the `:root` section of `styles.css` to change the color scheme.

### Contact Information

Update the contact section with your group's information in the "Contact Us" section of `index.html`.

---

**Last updated:** April 2024
