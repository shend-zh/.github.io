# Publish to GitHub Pages

The site is ready to publish as a static GitHub Pages site.

## Best URL

For a personal homepage at:

```text
https://YOUR-GITHUB-USERNAME.github.io/
```

create a public repository named exactly:

```text
YOUR-GITHUB-USERNAME.github.io
```

For a project-style URL, any repository name works. For example, a repository named
`website` would usually publish at:

```text
https://YOUR-GITHUB-USERNAME.github.io/website/
```

## Upload Through GitHub

1. Go to `https://github.com/new`.
2. Create a public repository.
3. Do not add a README, license, or `.gitignore` on GitHub.
4. Upload the contents of this folder, not the folder itself.
5. Commit the uploaded files.
6. Open the repository settings.
7. Go to Pages.
8. Under Build and deployment, choose:
   - Source: Deploy from a branch
   - Branch: `main`
   - Folder: `/root`
9. Save and wait for GitHub to publish the site.

## Upload Through Git

After creating the empty repository on GitHub, run:

```powershell
cd "C:\Users\User\Documents\Codex\2026-05-26\could-you-help-me-set-up"
git config user.name "Shend Zhjeqi"
git config user.email "YOUR-EMAIL@example.com"
git add .
git commit -m "Initial personal website"
git remote add origin https://github.com/YOUR-GITHUB-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

Then enable GitHub Pages from the repository settings using `main` and `/root`.
