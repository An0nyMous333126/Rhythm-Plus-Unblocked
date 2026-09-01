# Rhythm Plus Portfolio Deployment

This package is prepared for GitHub Pages. The source is the legacy V1 Rhythm Plus project.

## 1. Put the project on GitHub

Create a new **public** GitHub repository and upload the contents of this folder to the `main` branch.

## 2. Enable GitHub Pages

Open **Settings → Pages**. Under **Build and deployment**, choose **GitHub Actions**.

The included `.github/workflows/pages.yml` builds the project and publishes `dist/` automatically whenever you push to `main`.

## 3. Your game URL

After the workflow succeeds, GitHub will give you a URL similar to:

`https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`

## 4. About:blank launcher

Upload `launcher.html` to the same repository (or another static host). Its URL can be used like:

`https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/launcher.html?game=https%3A%2F%2FYOUR-USERNAME.github.io%2FYOUR-REPOSITORY%2F`

For Google Sites, use **Insert → Button** and set the button URL to that launcher URL.

The launcher opens a new blank tab and writes an iframe containing your deployed game into it. Browser popup blocking can prevent the new tab if the launcher is not opened directly by a user click.

## Important

The project uses the original Rhythm Plus V1 Firebase backend configuration. Do not remove the existing Firebase configuration if you want the application to retain its online functionality.
