# Doc Site (zudo-doc)

Astro + MDX documentation site. Port 4819.

## Content

- EN: `src/content/docs/` — default locale, no URL prefix
- JA: `src/content/docs-ja/` — `/ja/docs/...` URL prefix
- JA mirrors EN directory structure exactly

## MDX Frontmatter

```yaml
---
title: "Page Title"
description: "Brief description"
sidebar_position: 1
---
```

## Components (no import needed)

- `<Note>`, `<Tip>`, `<Info>`, `<Warning>`, `<Danger>` — admonitions
- `<HtmlPreview>` — interactive HTML/CSS/JS preview

## Typography

- Futura for page h1 titles and header site name (`font-futura` class)
- Noto Sans JP for body text
- Headings use font-weight 400 (normal), not bold
- Google Fonts loaded via layout `<head>`

## Settings

`src/config/settings.ts` — site name, description, header nav, footer, base path (`/pj/zudo-tauri`).
