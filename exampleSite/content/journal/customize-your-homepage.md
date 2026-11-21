---
title: "Customize the homepage and navigation"
date: 2026-11-21
description: "Change the Lux Mundi homepage copy and main navigation in Hugo configuration."
summary: "Edit the params and menu entries in hugo.toml to make the site your own."
---

The homepage hero is controlled by the `[params]` settings in your site's `hugo.toml`:

```toml
[params]
  description = "A concise description for search and browser metadata."
  eyebrow = "Independent film · Thoughtful storytelling"
  headline = "Stories that stay with you."
  intro = "Introduce your studio in one or two sentences."
  footer = "Independent stories, made with intention."
```

Add or rename navigation links using Hugo's menu configuration. The `pageRef` should match a content section or page in your site:

```toml
[menus]
  [[menus.main]]
    name = "Films"
    pageRef = "/projects"
    weight = 1
  [[menus.main]]
    name = "About"
    pageRef = "/about"
    weight = 2
  [[menus.main]]
    name = "Journal"
    pageRef = "/journal"
    weight = 3
```

Create the matching content folders, such as `content/about/_index.md` and `content/journal/_index.md`. Hugo orders menu items by `weight`; lower numbers appear first.
