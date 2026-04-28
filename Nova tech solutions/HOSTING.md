# Hosting the Nova Tech Support Website

This project is ready to publish as a static website on GitHub Pages.

## 1. Create a GitHub repository

1. Create a new repository on GitHub named `nova-tech-solutions`.
2. Push this project to the repository.

## 2. Deploy with GitHub Actions

The repository already includes a GitHub Actions workflow at `.github/workflows/deploy.yml`.

When you push to `main`, the workflow will:

- checkout the repository
- publish the site to the `gh-pages` branch
- deploy the website automatically

## 3. Access the website

After deployment, the public URL will be:

`https://<github-username>.github.io/nova-tech-solutions/`

Replace `<github-username>` with your GitHub username.

## 4. Local preview

Use a local server to preview the site with service worker support:

- `python -m http.server 8000`
- open `http://localhost:8000/index.html`

## 5. Notes

- If GitHub Pages is set to deploy from the `gh-pages` branch, the site will be available at the URL above.
- If needed, update the Pages settings in the repository to use the `gh-pages` branch.
