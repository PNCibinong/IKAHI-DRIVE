How to publish `2025_index.html` (quick steps)

Option A — GitHub Pages (recommended)
1. Create a new GitHub repository (public or private with Pages enabled).
2. Commit the files into the repo root (or `docs/`) — include:
   - `2025_index.html`
   - `2025_cleaned.md`
   - `2025_links.csv`
   - `2025_metadata.json`
3. In the repo, go to Settings → Pages and select the branch and folder (root or `/docs`) to publish.
4. After a few minutes your site will be available at `https://<your-username>.github.io/<repo>/2025_index.html`.

Quick commands (PowerShell):
```powershell
cd "path\to\folder"
git init
git add .
git commit -m "Add IKAHI index"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo>.git
git push -u origin main
```

Option B — Upload to any web host (FTP / cPanel)
- Upload the same files to a folder on your web host; then share the URL that points to `2025_index.html`.

Option C — Serve locally (for testing)
```powershell
# From folder containing 2025_index.html
python -m http.server 8000
# Then open http://localhost:8000/2025_index.html
```

Notes
- Keep the files together; links are relative (`2025_links.csv`, `2025_cleaned.md`, `2025_metadata.json`).
- If you want me to create a single ZIP ready to upload, tell me and I will bundle it.
- If you want me to commit to a GitHub repo for you, provide repo name and confirm you will grant access or share credentials (I cannot access your account automatically).
