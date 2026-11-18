# Golf Course AI Simulator — iPhone PWA

## GitHub Pages deployment

1. Create a **public** GitHub repository (for example `golf-course-ai-iphone`).
2. Upload the **contents of this folder** to the repository root (do not upload the parent folder itself).
3. Ensure the default branch is `main`.
4. Open **Settings → Pages** and set **Build and deployment → Source** to **GitHub Actions**.
5. Open the **Actions** tab and wait for **Deploy Golf AI to GitHub Pages** to complete successfully.
6. The site URL will be `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.
7. On iPhone, open that URL in Safari, tap Share → Add to Home Screen.

The repository and published Pages website are public. Do not upload personal or sensitive data.

## Included
- `index.html` and PWA manifest
- Service worker and app icons
- GitHub Actions workflow for automatic Pages deployment
- `.nojekyll`

## Current limitations
The current release is a mobile PWA prototype. Camera preview/recording is supported where iOS Safari permits it. It does not yet contain automatic golf-ball detection, trajectory tracking, validated distance measurement, true Orient GIS layers, cloud sync, or App Store native packaging.
