# Christine Nicole Tecson — Portfolio

A clean, modern, responsive personal portfolio website for Christine Nicole Tecson — Virtual Assistant, Graphic Designer, and Social Media Manager.

## Structure

```
.
├── index.html      # Page markup and content
├── style.css       # Design system + responsive styles
├── script.js       # Navigation, scroll effects, reveal animations
└── assets/
    ├── christine-photo.jpg              # Profile photo
    ├── Christine_Tecson_Resume.pdf      # Downloadable resume
    └── Wadhwani_Ignite_Certificate.pdf  # Downloadable certificate
```

## Running locally

No build step needed — it's plain HTML/CSS/JS.

1. Open the folder in any code editor.
2. Open `index.html` directly in a browser, **or** run a simple local server (recommended, so relative paths behave the same as on GitHub Pages):
   ```bash
   python3 -m http.server 8000
   ```
   Then visit `http://localhost:8000`.

## Deploying to GitHub Pages

1. Create a new GitHub repository (e.g. `christine-portfolio`).
2. Push all files in this folder to the repository's `main` branch, keeping the same folder structure (the `assets/` folder must stay alongside `index.html`).
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to "Deploy from a branch", choose the `main` branch and `/ (root)` folder, then save.
5. After a minute or two, your site will be live at:
   `https://<your-username>.github.io/<repository-name>/`

## Updating content later

- **Text content** (About, Skills, Projects, Experience, Certificates, Contact): edit directly inside `index.html` — each section is clearly commented.
- **Resume / Certificate files**: replace the PDFs in `assets/` with new files of the *same filename*, or update the filenames in `index.html` (search for `assets/Christine_Tecson_Resume.pdf` and `assets/Wadhwani_Ignite_Certificate.pdf`).
- **Photo**: replace `assets/christine-photo.jpg` with a new image of the same filename (recommended: a portrait-oriented photo, at least 800px wide).
- **Colors / fonts**: all design tokens (colors, spacing, radius, shadows) are defined as CSS variables at the top of `style.css` under `:root` — change them once and the whole site updates.

## Adding a new project card

Copy one `<article class="project-card">...</article>` block inside the `#projects` section in `index.html`, then update the title, description, tags, thumbnail color (`data-tone="blue|purple|rose|green"`), and date range.

## Credits

Fonts: [Poppins](https://fonts.google.com/specimen/Poppins) and [Inter](https://fonts.google.com/specimen/Inter) via Google Fonts.
