# Strojepis v brskalniku

This site runs your existing Strojepis DOS programs (`asdf`, `fdsa`, `fdsa2`) inside DOSBox compiled for the web. Anyone with the GitHub Pages link can open a DOS prompt and type the same commands.

## How to publish on GitHub Pages

Git is not required. You can upload the files in the browser.

1. Open [GitHub](https://github.com) and sign in.
2. Click **+** → **New repository**.
3. Name it `strojepis-web`.
4. Set it to **Public**.
5. Do **not** add a README (this folder already has one).
6. Click **Create repository**.
7. On the empty repo page, click **uploading an existing file**.
8. Drag these files from `C:\Users\Profesor\strojepis-web` into GitHub:
   - `index.html`
   - `strojepis.jsdos`
   - `README.md`
   - `.nojekyll` (this file may be hidden in File Explorer; enable "Hidden items" on the View tab if you do not see it)
   Do **not** upload `bundle-src` (that folder is only used to rebuild the DOS package).
9. Click **Commit changes**.
10. Open **Settings** → **Pages**.
11. Under **Build and deployment**, choose **Deploy from a branch**.
12. Branch: `main` (or `master`), folder: `/ (root)`.
13. Click **Save**.
14. After 1–2 minutes, open:

`https://YOUR-USERNAME.github.io/strojepis-web/`

Replace `YOUR-USERNAME` with your GitHub username.

## What visitors see

- A DOS screen with the Strojepis menu
- Type `asdf`, `fdsa`, or `fdsa2` and press Enter
- The `VAJE` exercise texts are already on the virtual C: drive

Click inside the black screen so the keyboard goes to DOS, not the web page.

## Rebuild the DOS package

If you change programs in `C:\Users\Profesor\Documents\DOSBoxPortable - z zvokom`, copy the `.EXE` files and the `VAJE` folder into `bundle-src`, then zip the **contents** of `bundle-src` (not the folder itself) into `strojepis.jsdos`. The zip must contain `.jsdos\dosbox.conf` at the top level.
