# CyberRoot

A single-file cybersecurity learning platform (frontend-only MVP demo). No build step, no backend — just `index.html`.

## Publish on GitHub Pages (5 minutes)

1. Create a new repo on GitHub (e.g. `cyberroot`).
2. Upload `index.html` (this file) to the repo root — either drag-and-drop on github.com, or:
   ```bash
   git init
   git add index.html README.md
   git commit -m "CyberRoot MVP"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Source → Deploy from a branch → `main` / `(root)` → Save**.
4. Your site goes live at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

## Notes
- All data (progress, XP, quiz scores, CTF flags, notes/tools added via Admin) is stored in each visitor's browser via `localStorage` — there is no shared database. Different visitors will not see each other's data.
- This is a frontend demo. A production build would need a real backend (auth, database, admin API) as described in the app's own Admin panel.
