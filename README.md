# Iqra Ali — Academic Portfolio Website

A responsive single-page academic portfolio based on Iqra Ali's CV.

## Included sections

- Hero / academic profile
- About
- Research interests
- Selected publications
- Research and industry experience
- Education
- Academic service and community leadership
- Awards and honours
- Technical skills
- Selected talks and tutorials
- Contact details
- Responsive mobile navigation
- Light/dark theme toggle
- Basic SEO and Schema.org metadata

## Files

```text
.
├── index.html
├── styles.css
├── script.js
├── assets/
│   └── favicon.svg
└── README.md
```

## Publish with GitHub Pages

### Option 1 — Personal website

1. Create a GitHub repository named:

   ```text
   YOUR-GITHUB-USERNAME.github.io
   ```

2. Upload all files in this folder to the repository root.

3. Commit and push the files.

4. Open **GitHub → Repository → Settings → Pages**.

5. Under **Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/(root)**

6. Your site will appear at:

   ```text
   https://YOUR-GITHUB-USERNAME.github.io/
   ```

### Option 2 — Push from Terminal

```bash
cd iqra-ali-github-website
git init
git add .
git commit -m "Create academic portfolio website"
git branch -M main
git remote add origin https://github.com/YOUR-GITHUB-USERNAME/YOUR-GITHUB-USERNAME.github.io.git
git push -u origin main
```

Then enable GitHub Pages from the repository settings if it is not enabled automatically.

## Recommended edits before publishing

### Add your GitHub profile
Add a GitHub link next to Google Scholar and LinkedIn in `index.html` once you decide which profile you want to show.

### Add a profile photo
The current design intentionally uses an `IA` monogram so the site works immediately without an image.

To use a photo instead:

1. Put the image in `assets/profile.jpg`.
2. Replace the `.avatar` block in `index.html` with:

```html
<div class="avatar photo-avatar">
  <img src="assets/profile.jpg" alt="Iqra Ali" />
</div>
```

3. Add this to `styles.css`:

```css
.photo-avatar {
  overflow: hidden;
}

.photo-avatar img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```

### Add your CV PDF
Place your PDF at:

```text
assets/Iqra_Ali_CV.pdf
```

Then add a button or link such as:

```html
<a href="assets/Iqra_Ali_CV.pdf" target="_blank">Download CV</a>
```

## Notes

- The website uses no external frameworks and can be hosted directly on GitHub Pages.
- All content is editable in `index.html`.
- Colours and spacing are controlled in `styles.css`.
- The theme toggle is stored in the visitor's browser via `localStorage`.
