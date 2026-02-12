# Valentine Frontend

Yes — this project is **frontend-only**. It is a single-page static site (`index.html`) with no backend.

## Deploy on GitHub Pages

This repository includes a GitHub Actions workflow at `.github/workflows/deploy-pages.yml`.

### 1) Push this repository to GitHub

```bash
git remote add origin <your-github-repo-url>
git push -u origin <your-branch>
```

### 2) Enable Pages in GitHub settings

- Open **Settings → Pages**
- Under **Build and deployment**, set **Source** to **GitHub Actions**

### 3) Trigger deployment

- Merge/push to `main` or `master`, or
- Run the workflow manually from **Actions → Deploy static site to GitHub Pages → Run workflow**

### 4) Live URL

Once deployed, GitHub Pages will publish at:

- `https://<username>.github.io/<repo>/`


## Couple photo used after clicking YES

- The current couple photo is embedded directly in `index.html` as a `data:image/jpeg;base64,...` source for `#coupleImage` (no binary asset file required).
- To replace it later, update the `src` of `#coupleImage` with your new image URL or another data URI.
