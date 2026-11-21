# Lux Mundi

[![Deploy with GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-222?logo=github)](https://github.com/poonchavez/lux-mundi/actions/workflows/hugo.yml)
[![Deploy with GitLab Pages](https://img.shields.io/badge/Deploy-GitLab%20Pages-fc6d26?logo=gitlab&logoColor=white)](https://docs.gitlab.com/user/project/pages/)
[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fpoonchavez%2Flux-mundi)
[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/poonchavez/lux-mundi)

Lux Mundi is a cinematic, responsive Hugo theme for independent filmmakers, production studios, and creative portfolios. It pairs an editorial type system and warm gold accents with a dark, film-inspired palette.

## Quick start

Install the theme in your Hugo site's `themes/lux-mundi` directory, then set `theme = "lux-mundi"` in `hugo.toml`. The `exampleSite` directory includes a working starter configuration and sample pages.

```toml
title = "Lux Mundi"
theme = "lux-mundi"

[params]
  description = "Independent films and stories made with intention."
  eyebrow = "Independent film · Thoughtful storytelling"
  headline = "Stories that stay with you."
  intro = "An independent production studio creating films rooted in curiosity, craft, and the human experience."

[menus]
  [[menus.main]]
    name = "Films"
    pageRef = "/projects"
  [[menus.main]]
    name = "About"
    pageRef = "/about"
```

To build the bundled example site from this theme repository, run:

```sh
hugo --source exampleSite --themesDir .. --theme .
```

When using the theme in another Hugo site, run `hugo` from that site's root instead.

## Adding a project

Create a page under `content/projects/`, for example `hugo new content projects/my-film.md`. Add front matter such as:

```yaml
---
title: "My Film"
subtitle: "A short description"
year: "2026"
category: "Documentary"
image: "poster.jpg"
imageAlt: "A still from My Film"
externalURL: "https://example.org/my-film"
---

Write a project description here.
```

Place project images beside the page bundle and use page-bundle paths, or use an image path from `static/`. Project cards appear on the homepage and the project listing page. Set `draft: false` or publish the page to include it.

## Theme features

- Responsive homepage, project listing, project details, and general content layouts
- Page-bundle and static image support
- Accessible skip link, semantic landmarks, and reduced-motion support
- Customizable studio copy through `params`
- No JavaScript dependencies

The theme imports DM Sans and Playfair Display from Google Fonts, with local system fallbacks.
