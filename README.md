# Yun Li — academic homepage

Trilingual (EN / 中文 / 日本語) academic homepage built with [Hugo](https://gohugo.io/).

## Local preview

```bash
hugo server -D
# → http://localhost:1313/
```

## Build

```bash
hugo --gc --minify
# output → public/
```

## Editing content

- `content/<lang>/_index.md` — About page (homepage)
- `content/<lang>/publications/*.md` — one file per publication
- `content/<lang>/news/*.md` — one file per news item
- `content/<lang>/cv.md` — full CV
- `content/<lang>/contact.md` — contact info
- `hugo.toml` — site config, author identity, social links

## Assets

- `static/img/avatar.jpg` — profile photo
- `static/img/utokyo.png`, `tieriv.png` — affiliation logos
- `static/css/style.css` — site styling

## Deploy

Built for **Cloudflare Pages**:

| Setting | Value |
|---|---|
| Framework preset | Hugo |
| Build command | `hugo --gc --minify` |
| Build output directory | `public` |
| Environment variable | `HUGO_VERSION = 0.139.0` |

Update `baseURL` in [hugo.toml](./hugo.toml) once the deploy URL is known.
