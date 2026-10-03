# Pranav Baraskar — Performance Marketer Portfolio

A single-page portfolio site: About, Proof (real dashboards), Expertise, Automation, Video creatives, and Contact — with embedded images/videos so it works as a fully static site (no build step, no external assets besides Google Fonts).

## Files
- `index.html` — page structure/content
- `style.css` — all styling
- `script.js` — carousels, tabs, lightbox, reveal animations, embedded video/image data

## Run locally
Just open `index.html` in a browser, or serve the folder:
```
python3 -m http.server 8000
```
then visit http://localhost:8000

## Push to GitHub
```bash
cd portfolio-site
git init
git add .
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

## Host for free (optional)
Since it's fully static, you can deploy it as-is to:
- **GitHub Pages**: Settings → Pages → Deploy from branch → `main` → `/ (root)`
- **Netlify** or **Vercel**: drag-and-drop the folder, or connect the GitHub repo

Note: `script.js` is large (~12 MB) because the video creatives are embedded as base64. That's fine for GitHub/Pages, Netlify, Vercel.
