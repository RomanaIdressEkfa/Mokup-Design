# Proof Sheet

A small browser tool that turns two or more website screenshots into a clean
side-by-side comparison card, for portfolio use (Fiverr, LinkedIn, anywhere).

- Upload any number of screenshots, reorder them, remove any.
- Pick a background from 14 presets or set your own two-color gradient.
- Every card ends up the exact same width and height. A taller screenshot is
  cropped automatically (you choose whether it keeps the top, middle, or
  bottom) — nothing is ever stretched or squeezed.
- "Split one tall screenshot into panels" slices a single long page screenshot
  into equal pieces and lays them out side by side.
- Everything runs in your browser. No upload, no server, no account.

It is one file: `index.html`. No build step, no dependencies to install.

## Use it right now

Just open `index.html` in a browser (double-click it, or drag it into a
browser window). That's the whole setup.

## Put it on GitHub Pages (free hosting, your own link)

1. Create a new GitHub repository (public or private — Pages needs a public
   repo on the free plan, or a private one if you have GitHub Pro/Team).
2. Upload this folder's `index.html` to the repository (drag-and-drop on
   github.com works, or use git: see below).
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose `main` and folder `/ (root)`, then **Save**.
6. GitHub shows your live URL after a minute or two, something like
   `https://<your-username>.github.io/<repo-name>/`.

### Using git from the command line instead

```
git init
git add index.html README.md
git commit -m "Add Proof Sheet"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

Then do steps 3–6 above.

## Notes

- Needs a modern browser (Chrome, Edge, Firefox, Safari — anything from the
  last few years). It uses `createImageBitmap` and `<canvas>`, both standard.
- The "Download" button saves a PNG straight to your Downloads folder, the
  normal way any website download works.
- Nothing is sent anywhere — all image processing happens on your own device.
