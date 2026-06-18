# Blog setup &mdash; GitHub Pages deployment

This is a minimal Jekyll site, pre-configured for GitHub Pages with zero build-step setup required on your end.

## 1. Create the repository

Create a new GitHub repo named exactly `rohitchandramouli.github.io` (replace with your actual GitHub username if different &mdash; the repo name must exactly match `<username>.github.io` for GitHub Pages to auto-serve it at the root domain).

## 2. Push these files

```bash
git init
git add .
git commit -m "feat: initial blog scaffold with first post"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
git push -u origin main
```

## 3. Enable Pages

In the repo on GitHub: Settings &rarr; Pages &rarr; Source &rarr; select `Deploy from a branch` &rarr; Branch: `main`, folder `/ (root)` &rarr; Save.

GitHub will build and publish the site automatically within a minute or two. It will be live at `https://<your-username>.github.io`.

## 4. Update `_config.yml`

Before pushing, edit `_config.yml`:
- Set `url` to your actual GitHub Pages URL (already set assuming your username is `rohitchandramouli` &mdash; double-check it matches).
- Set `author.github` to your actual GitHub username if different.

## 5. Writing new posts

Every new post is a markdown file in `_posts/`, named exactly `YYYY-MM-DD-some-title.md`, with this header (called front matter) at the top:

```markdown
---
layout: post
title: "Your Post Title"
date: 2026-06-25
tags: [week-1, python]
---

Your post content in regular markdown starts here.
```

Commit and push that one file — no rebuild step needed locally, GitHub does it for you automatically every time you push to `main`.

## 6. Local preview (optional)

If you want to preview before pushing, install Ruby + Bundler, then:

```bash
bundle install
bundle exec jekyll serve
```

Visit `http://localhost:4000`. Not required &mdash; you can also just push and check the live site after a minute, which is simpler if you don't want to install a local Ruby environment.

## Folder structure reference

```
.
├── _config.yml        # site settings (title, description, url)
├── _layouts/
│   ├── default.html   # base HTML wrapper, header/footer, all CSS
│   └── post.html      # post-specific title/meta wrapper
├── _posts/             # every blog post lives here, one .md file each
├── about.md            # the About page
├── index.html          # the homepage (lists all posts automatically)
└── Gemfile             # tells GitHub Pages which plugins to use
```

You should essentially never need to touch `_layouts/` or `_config.yml` again after initial setup &mdash; from here on, writing a new post is just adding one new file to `_posts/`.
