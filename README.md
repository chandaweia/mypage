# Personal academic homepage

A static site (plain HTML + CSS, no build step) hosted with GitHub Pages.

## Structure

- `index.html` — home: photo, bio, contact links, news, research summary
- `publications.html` — publications grouped by type
- `research.html` — research projects and skills
- `css/style.css` — the only stylesheet
- `images/` — profile photo (`profile.svg` is a placeholder; replace with `profile.jpg` and update the `<img>` in `index.html`)
- `assets/` — CV (`cv.pdf`) and other files
- `.nojekyll` — tells GitHub Pages to serve the files as-is

## Deploying with GitHub Pages

1. Push this branch to GitHub and merge it into `main`.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, set Source to **Deploy from a branch**,
   choose `main` and the `/ (root)` folder, then save.
4. The site appears at `https://chandaweia.github.io/mypage/` within a minute or two.
5. The `CNAME` file sets the custom domain `cuidi.net`; DNS at the registrar must point
   the apex to GitHub Pages A/AAAA records and `www` to `chandaweia.github.io`.

To serve at `https://chandaweia.github.io/` instead, rename the repository to
`chandaweia.github.io`. A custom domain can be added on the same Pages settings page.

## Editing

Every page is hand-written HTML. To add a publication, copy one `<li>` block in
`publications.html` and edit it. To add news, add a `<li>` to the list in `index.html`.
