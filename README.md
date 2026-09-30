# Brian Kibet - Portfolio & Blog

Personal portfolio and blog built with [Jekyll](https://jekyllrb.com/) and hosted on GitHub Pages at
<https://bryanarapkoech.github.io/KibetArapKoech.github.io/>.

## Structure

- `index.md` - single-page portfolio (about, services, work)
- `blog/index.md` - blog index; posts live in `_posts/`
- `about.markdown` - about page
- `_layouts/` - `default` (pages) and `post` (blog posts)
- `_includes/` - shared nav, footer and menu script
- `css/` - hand-written styles
- `public/assets/` - images

## Run locally

```sh
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000/KibetArapKoech.github.io/> (the `baseurl` in `_config.yml` applies locally too).

## Add a blog post

Create `_posts/YYYY-MM-DD-Title.markdown` with front matter:

```yaml
---
layout: post
title: "Post title"
date: YYYY-MM-DD HH:MM:SS +0300
categories: Topic
excerpt: One-line summary shown on the blog index.
---
```
