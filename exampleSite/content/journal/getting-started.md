---
title: "Getting started with Lux Mundi"
date: 2026-11-21
description: "Install the theme in a Hugo site and preview your first Lux Mundi pages."
summary: "Install Lux Mundi, configure the theme, and run a local preview of your site."
---

Lux Mundi is a Hugo theme. To use it, you need a Hugo site and the theme files inside that site.

## Install the theme

From your site's root, add Lux Mundi as a Git submodule:

```sh
git submodule add https://github.com/poonchavez/lux-mundi.git themes/lux-mundi
```

If you downloaded the theme instead, place its folder at `themes/lux-mundi`.

## Configure your site

In your site's `hugo.toml`, set the theme and add your studio's homepage copy:

```toml
title = "Your Studio"
theme = "lux-mundi"

[params]
  description = "Independent films and stories made with intention."
  eyebrow = "Independent film · Thoughtful storytelling"
  headline = "Stories that stay with you."
  intro = "A short introduction to your studio."
```

Set `baseURL` to your site's public URL when preparing a production build.

## Preview the site

Run Hugo from the site root:

```sh
hugo server
```

Open the local URL printed by Hugo. The bundled `exampleSite` in the Lux Mundi repository is also ready to preview from the theme checkout:

```sh
hugo server --source exampleSite --themesDir .. --theme .
```
