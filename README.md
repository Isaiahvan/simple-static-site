# Simple Static Site

This repository is a minimal static site scaffold you can deploy with Git.

Quick local test

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

Deploy to GitHub Pages

1. Create a GitHub repository (empty) via the website or `gh repo create`.
2. Add the remote and push:

```sh
git remote add origin git@github.com:YOUR_USER/YOUR_REPO.git
git branch -M main
git push -u origin main
```

3. In the repository Settings → Pages, choose branch `main` (or `gh-pages`) and the root folder to publish.

Deploy to Netlify

1. Create a Netlify site and connect your GitHub repository, or use the Netlify CLI.

Optional automation

- Add a GitHub Actions workflow to build/publish on push if you later add a build step.
