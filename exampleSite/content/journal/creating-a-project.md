---
title: "Create a project page"
date: 2026-11-21
description: "Add a film or project to the homepage and portfolio listing."
summary: "Create a page bundle with project details and an optional poster image."
---

Project pages live in `content/projects/`. Give each project its own folder so its image and content stay together:

```text
content/projects/my-film/index.md
content/projects/my-film/poster.jpg
```

Add front matter to `index.md`:

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

Write the project description here.
```

The project appears in the homepage selection and the Films listing. The image path is relative to the page bundle. You can omit `image` to show the theme's placeholder, or use an image under `static/` with a site-root path such as `/images/my-film.jpg`.

To create a project from the terminal, run `hugo new content projects/my-film/index.md` from your site root. Review the generated front matter and set `draft: false` or remove `draft` before publishing.
