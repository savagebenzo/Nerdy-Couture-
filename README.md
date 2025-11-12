Needy Couture
===============

This is a small static site (single-file) for Needy Couture. It includes a simple client-side UI for collections, fabrics, a demo cart, an image manager, and price USD/NGN synchronization.

How to publish to GitHub

1. Create a repository on GitHub (e.g., `needy-couture`).
2. On your machine in this project folder run the commands below (replace <remote-url> with your repository URL):

```powershell
cd 'c:\Users\user\OneDrive\Desktop\Nerdy Couture'
# if not already initialized
git init
git add .
git commit -m "Initial site commit"
# create main and gh-pages branches
git branch -M main
git checkout -b gh-pages
# push (replace <remote-url> with your GitHub repo HTTPS/SSH URL)
git remote add origin <remote-url>
git push -u origin gh-pages
```

3. On GitHub, go to the repository Settings → Pages and set the source to the `gh-pages` branch (root) — the site will be served at `https://<username>.github.io/<repo>`.

Notes
- This project uses localStorage for demo cart and image overrides. No backend is included.
- If you prefer using the `main` branch for Pages, push `main` and select it in Pages settings.

If you want, I can also:
- Create a GitHub Actions workflow to deploy automatically, or
- Add a small script to publish directly from this repo (requires remote credentials).
