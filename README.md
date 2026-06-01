# guowei-uga.github.io

## Overview

This repository hosts the academic website for Guo-Wei Wei at the University of Georgia. The site is built with Jekyll using the al-folio theme and deployed with GitHub Pages.

Production site: https://guowei-uga.github.io

## Getting Started

Clone the repository and install the Ruby dependencies:

```bash
bundle install
```

Run the site locally:

```bash
bundle exec jekyll serve --host 127.0.0.1 --port 4001
```

Then open http://127.0.0.1:4001/ in a browser.

## Local Development

Use the local server while editing pages, data files, mirrored HTML, or assets. Rebuild manually when you only need to check that Jekyll can generate the site:

```bash
bundle exec jekyll build
```

The generated site is written to `_site/`, which should not be edited by hand.

## Deployment

This is a personal/organization GitHub Pages site. Keep these deployment settings:

- Repository name: `guowei-uga.github.io`
- `_config.yml` `url`: `https://guowei-uga.github.io`
- `_config.yml` `baseurl`: empty
- Deployment branch: `master`

After making changes, commit and push:

```bash
git add -A
git commit -m "Describe the change"
git push origin master
```

GitHub Pages/Actions will deploy the site after the push. Deployment can take a few minutes to become visible.

## Content Notes

Common maintenance locations:

- `_pages/`: main site pages such as About, Publications, Talks, Teaching, Resources, and Positions.
- `_data/`: structured content lists such as research interests, talks, teaching, and publications-related data.
- `assets/html/`: local mirrored HTML pages, including former MSU-hosted pages and Word-converted archival pages.
- `assets/css/`: custom styles, including mirror-page styles.
- `assets/pdf/`: local PDF copies used by the site.

When replacing MSU-hosted resources, keep local copies under `assets/html/`, `assets/pdf/`, or another appropriate `assets/` subfolder and update site links to point to the local copy.

## FAQ

### How do I run the site locally?

Run:

```bash
bundle exec jekyll serve --host 127.0.0.1 --port 4001
```

Then open http://127.0.0.1:4001/.

### Why does the deployed site take time to update?

GitHub Pages deployment is asynchronous. After pushing to `master`, wait for the Actions/Pages deployment to finish and allow a few minutes for the public site to refresh.

### Why is `baseurl` empty?

This repository is deployed as `https://guowei-uga.github.io`, not as a project subpath. For this type of GitHub Pages site, `baseurl` should stay empty.

### Where are mirrored HTML files stored?

Mirrored and converted pages are stored under `assets/html/`. Publication mirrors are under `assets/html/publications/`; talks, seminars, and conference mirrors are under `assets/html/talks/`; resource mirrors are under `assets/html/repositories/`.

### How should publication or resource links be updated?

Prefer local copies for former MSU-hosted resources. Download or convert the source file into the relevant `assets/` folder, then update the link on the visible site page to point to that local path.

### What should I check before pushing?

At minimum, run:

```bash
bundle exec jekyll build
```

Also preview important changed pages locally, especially mirrored HTML pages and publication/resource links.

## Theme Credit

This site is based on the al-folio Jekyll theme.

Website setup and migration by [Rui Wang](https://github.com/wangru25).
