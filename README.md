# Asela Hevapathige — personal website

A static, multi-page academic profile. No package installation, database or build command is required.

## Publish on GitHub Pages

1. Sign in to GitHub and create a **public** repository named `YOUR_USERNAME.github.io`, replacing YOUR_USERNAME with your actual GitHub username.
2. Extract the ZIP and upload its contents to the repository root. `index.html` must be at the root, not inside an extra folder. Commit the files to `main`.
3. Open the repository's **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
5. Select **main** and **/ (root)**, then select **Save**.
6. When the Pages deployment completes, the site will be available at `https://YOUR_USERNAME.github.io/`.

If you prefer an ordinary repository name, the same files also work at `https://YOUR_USERNAME.github.io/REPOSITORY_NAME/`. Internal links are relative to support both arrangements.

## Edit the website

Edit the HTML files directly and commit the changes. GitHub Pages will republish them. Colours, spacing and responsive layouts are in `style.css`.

- `index.html`: About page and photo placeholder
- `research.html`: research areas
- `publications.html`: selected publications
- `experience.html`: experience overview
- `education.html`, `teaching.html`, `research-experience.html`, `industry.html`, `service.html`, `awards.html`: experience pages
- `contact.html`: contact information
- `404.html`: not-found page

## Add your photograph

1. Place your photo in the repository root as `profile.jpg`.
2. In `index.html`, replace the entire `<div class="photo-placeholder" ...>...</div>` with:

```html
<img class="profile-photo" src="profile.jpg" alt="Asela Hevapathige">
```

3. Add this to the end of `style.css`:

```css
.profile-photo {
  display: block;
  width: 100%;
  max-width: 240px;
  aspect-ratio: 4 / 5;
  object-fit: cover;
  border: 1px solid #cbdaea;
  border-top: 4px solid #467ba7;
}
@media (max-width: 600px) {
  .profile-photo { max-width: 145px; }
}
```

No API keys or credentials are required. This package contains the public website files only.
