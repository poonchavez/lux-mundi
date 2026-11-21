---
title: "Build and publish your site"
date: 2026-11-21
description: "Build a production-ready site with Hugo and understand the example deployment workflow."
summary: "Generate the static site locally, then connect your repository to a hosting provider."
---

Build your site from its root directory:

```sh
hugo --minify
```

Hugo writes the generated site to `public/`. Preview the site locally with:

```sh
hugo server
```

The Lux Mundi repository includes a GitHub Actions workflow that builds the bundled example site and publishes it with GitHub Pages. For a site using the theme, copy or adapt that workflow to build from your own site root. On other hosting services, configure the build command as `hugo --minify` and publish directory as `public/`.

For a local build of the theme repository's example site, use:

```sh
hugo --source exampleSite --themesDir .. --theme . --minify
```
