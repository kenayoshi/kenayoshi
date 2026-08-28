# Ken A. Yoshida — Portfolio Site

A single-file static site (`index.html`, CSS and JS inline — no build step, no dependencies besides two Google Fonts loaded via CDN).

## Before you publish

- **GitHub link**: search `index.html` for `add your username here` (two spots: hero links and the Contact pinout) and swap in your real GitHub profile URL.
- **Phone number**: left off on purpose since a GitHub repo is far more scraped/indexed than a Google Site. Add a line in the Contact section (`<div class="pin">` block) if you want it public.
- **Status pill**: currently reads "Class of 2029" — update the wording in the `.status-pill` div in the hero if you'd rather flag open-to-work/internship status.

## Deploy with GitHub Pages (no local setup needed)

1. Go to [github.com/new](https://github.com/new) and create a repository. Name it `<your-username>.github.io` if you want it at the root of your GitHub domain (e.g. `kenyoshida.github.io`) — any other name works too, it'll just live at `<your-username>.github.io/<repo-name>`.
2. On the new repo's page, click **uploading an existing file**, drag in `index.html` (and this `README.md` if you want), and commit.
3. Go to **Settings → Pages** in the repo.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**, pick the `main` branch and `/ (root)` folder, then **Save**.
5. GitHub will build the site in a minute or two and show you the live URL at the top of that same Pages settings page.

## Deploy from the command line instead

```bash
git init
git add index.html README.md
git commit -m "Add portfolio site"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

Then enable Pages the same way as step 3–5 above.

## Editing later

Everything is in `index.html` — content, CSS (in the `<style>` block), and the one small reveal-on-scroll script (in the `<script>` block at the bottom). No build tools, so any text editor + a reload of the page is the whole workflow.
