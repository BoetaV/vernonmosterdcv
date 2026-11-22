# Vernon Mosterd · Online CV

One-page CV site. Pure HTML and CSS, so there is no build step.

| File | What it is |
|---|---|
| `index.html` | The online CV: WebGL (Three.js) floating dot-sphere hero, CSS 3D skills cube, draggable tech sphere, 3D project ring, tilt and glare cards, gyroscope contact. Blue, navy and red theme. Three.js loads from the jsDelivr CDN. |
| `Vernon-Mosterd-CV.pdf` | Two-page A4 PDF, linked from the site |
| `cv-print.html` | Source of the PDF. Edit it, then print it again (see below) |

## Publish on GitHub Pages

1. The repository is `BoetaV/vernonmosterdcv` (public).
2. Upload the contents of this folder (not the folder itself) to the repository.
3. Go to **Settings → Pages**. Set the source to **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. After about a minute the site is live at `https://boetav.github.io/vernonmosterdcv/`.

## Rebuild the PDF after edits

```powershell
& "C:\Program Files\Google\Chrome\Application\chrome.exe" --headless=new --no-pdf-header-footer --print-to-pdf="Vernon-Mosterd-CV.pdf" "$PWD\cv-print.html"
```
