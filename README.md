# Anastasios Fotiadis — academic website

Personal academic website at **https://anastasis-dev97.github.io**, built with Jekyll and al-folio v1.

## Local development

Use Ruby 3.3 and Bundler 2.5.23:

```bash
gem install bundler -v 2.5.23
bundle install
bundle exec jekyll serve
```

Open `http://localhost:4000/`. Run `JEKYLL_ENV=production bundle exec jekyll build` to generate `_site/`.

## Deployment

The workflow `.github/workflows/deploy.yml` builds and publishes on pushes to `main`. In **Settings → Pages → Build and deployment**, the source must be **GitHub Actions**.

The configuration uses `url: https://anastasis-dev97.github.io` and an empty `baseurl`. The old `/index.html` URL continues to work, `/research.html` redirects to `/research/`, and the contact section is at `/#contact`.

## Editing content

| Content | File |
|---|---|
| Identity, canonical URL, features | `_config.yml` |
| About and contact | `_pages/about.md` |
| Research and work in preparation | `_pages/research.md` |
| Talks and conferences | `_data/talks.yml`, `_data/conferences.yml` |
| Teaching | `_data/teaching.yml` |
| Homepage education history | `_data/education.yml` |
| Academic CV | `_data/cv.yml` |
| Profile photo shown on the site | `assets/img/Anastasios-Fotiadis.webp` |
| Layout refinements | `_sass/_site.scss` |

The original full-resolution photograph remains in `DSCF4467.jpg`. The website uses a smaller WebP version with the full composition preserved.

The CV is maintained separately from the other data files. Update the corresponding CV entries when changing education, teaching, or talk information.

The contact email retains its original obfuscated form. The contact-vector-fields paper is explicitly marked **In preparation**.

## Theme maintenance

Theme and plugin versions are pinned in `Gemfile` and `Gemfile.lock`. `assets/css/main.scss` retains the upstream imports and adds `_sass/_site.scss`; this override is tracked in `.al-folio-overrides.yml`.

When upgrading the theme, run:

```bash
bundle exec al-folio upgrade audit
bundle exec al-folio upgrade overrides audit
```

Third-party Jekyll plugins load before `al_folio_core` so that theme-aware cache handling is installed correctly. No Node/npm, Docker, Python, or ImageMagick build step is needed for this site.

## Restoring the previous website

The original website is saved on the `backup-before-al-folio-2026-10-23` branch at commit `b849062ada772c0c9850058615cd632dd08160df`.

To publish that original website again, open **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, select **backup-before-al-folio-2026-10-23** and **/ (root)**, and save. This keeps the al-folio source on `main` available if you want to return to it later.

See `MIGRATION.md` for the content migration notes and al-folio's MIT license in `LICENSE`.
