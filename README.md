# erikwibbels.github.io

Personal academic website for Erik Wibbels. Plain HTML/CSS, no build step — works directly with GitHub Pages.

## Publishing this to GitHub Pages

1. Create a new repository on GitHub named exactly `ErikWibbels.github.io` (this special name makes GitHub
   Pages serve it at the root domain `https://erikwibbels.github.io`). You can also use any other repo name —
   e.g. `personal-site` — the site will just live at `https://erikwibbels.github.io/personal-site/` instead.
2. On your computer, unzip this folder, then from inside it run:

   ```
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/ErikWibbels/ErikWibbels.github.io.git
   git push -u origin main
   ```

3. On GitHub, go to the repo's **Settings → Pages**, and under "Build and deployment" set Source to
   **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
4. Within a minute or two your site will be live at the URL GitHub shows on that Pages settings screen.

## Updating the site later

Edit the HTML files directly (no build tools required), then:

```
git add .
git commit -m "Update site"
git push
```

GitHub Pages will redeploy automatically within a minute or two.

## Structure

```
index.html                       Home
research.html                    Research (published work)
research/working-papers.html     Working papers
teaching.html                    Teaching overview
teaching/psci1102/               PSCI 1102 course site (Home / Syllabus / Schedule)
policy.html                      Policy Work
cv.html                          Link to CV
css/style.css                    Shared stylesheet
```
