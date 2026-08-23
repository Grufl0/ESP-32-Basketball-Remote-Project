# ESP-32 Basketball Remote Project

## CourtSync Data Viewer

`index.html` is a self-contained, static web page that renders a CourtSync
game (a virtual LED scoreboard, player stat tables, and an event history)
from pasted CourtSync export data. It requires no build step or backend —
it's plain HTML/CSS/JS.

Paste either the raw BLE notification lines (e.g. copied from nRF Connect)
or a full Serial Monitor dump into the "Paste data" box and click **Parse**.

### Publishing on GitHub Pages

This repo includes a GitHub Actions workflow
(`.github/workflows/deploy-pages.yml`) that deploys `index.html` to GitHub
Pages automatically on every push to `main`.

To turn it on (one-time setup):

1. Merge this branch into `main`.
2. In the repository, go to **Settings → Pages**.
3. Under **Build and deployment → Source**, select **GitHub Actions**.
4. Push to `main` (or re-run the workflow from the **Actions** tab) to
   trigger a deployment.

Once enabled, the site will be publicly available at:

```
https://grufl0.github.io/ESP-32-Basketball-Remote-Project/
```
