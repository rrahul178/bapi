# BAPI Website (Static, GitHub Pages ready)

Full multi-page site for **Bangladesh Association of Pharmaceutical Industries (BAPI)** —
Home, About, Notices, Publications, Events, Contact. Plain HTML/CSS/JS, no build step.

## Structure
```
bapi-website/
├── index.html
├── about.html
├── notices.html
├── publications.html
├── events.html
├── contact.html
├── css/style.css
└── js/script.js
```

## What's placeholder and needs real content before launch
- Leadership names (President, CEO, ED) on about.html
- Real notices/circulars, publications, and events (currently sample entries)
- Phone number, official email address in contact.html and footers
- Member counts / stats on the homepage
- Contact form has no backend — either wire it to Formspree/Getform, or a simple
  server endpoint. Right now submitting just shows a placeholder message.

## Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g. `bapi-website`).
2. Push these files to the `main` branch:
   ```bash
   cd bapi-website
   git init
   git add .
   git commit -m "Initial BAPI website"
   git branch -M main
   git remote add origin https://github.com/<your-username>/bapi-website.git
   git push -u origin main
   ```
3. In the repo on GitHub: **Settings → Pages → Source** → select `main` branch,
   `/ (root)` folder → **Save**.
4. GitHub will publish the site at:
   `https://<your-username>.github.io/bapi-website/`
5. (Optional) Add a custom domain later under **Settings → Pages → Custom domain**
   once BAPI has one to point at it.

## Local preview
Just open `index.html` in a browser — no server needed. For live-reload while
editing, you can also run `python3 -m http.server` from inside the folder and
visit `http://localhost:8000`.
