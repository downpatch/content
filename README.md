# Downpatch Content Repository

This repository contains all markdown content for downpatch.com. The application pulls this repo directly and renders the pages at runtime.

The goal of this repo is:
- Keep content fully open source
- Keep structure simple
- Make guides easy to edit
- Avoid hidden logic inside the app

## How Content Sync Works
The k3s deployment runs the application in Kubernetes.
The content repository is:

- Cloned on container startup
- Refreshed hourly

This means:

- Pushing to `main` here will go live on the hour.

## Folder Structure

All guides live under:

```
guide/
```
Example:

```
guide/
  halo/
    index.md
    toc.yml
    haloreach/
      index.md
      levels.md
```
Rules:

- Every folder must contain an `index.md`
- Nested folders are allowed
- URLs are based on folder structure
- `index.md` becomes the folder root page

## Basic Frontmatter

Each markdown file must start with YAML frontmatter.

Recommended fields:

```yaml
---
title: Halo: Reach
nav_title: Halo: Reach
description: Getting started with Halo Reach speedrunning.

square_image: square.webp
og_image: og.webp

leaderboard: https://haloruns.com
discord: https://haloruns.com/discord

noindex: false
---
```

Field explanation:

- `title` — Main page title
- `nav_title` — Optional shorter title for sidebar
- `description` — Used for meta description + preview text
- `square_image` — Used on the game search page
- `og_image` — Used for social previews
- `leaderboard` — Optional external link
- `discord` — Optional external link
- `noindex` — If true, page will not appear in sitemap

## TOC Format (toc.yml)

Each folder can define its navigation using a `toc.yml`.

Example:

```yaml
- name: "Overview"
  href: index.md

- name: "Livesplit"
  href: livesplit.md

- name: Games
  items:
    - name: "Halo: Combat Evolved"
      href: haloce/index.md
    - name: "Halo 2"
      href: halo2/index.md
    - name: "Halo 3: ODST"
      href: halo3odst/index.md
```

Rules:

- `name` — Display text in sidebar (Value must be in quotations)
- `href` — Relative path to markdown file
- `items` — Nested navigation group
- Indentation must use spaces (not tabs)

If no `toc.yml` exists, the folder will still work, but navigation will be limited.

## URL Behaviour

- `/guide/folder/index.md` becomes `/guide/folder` in the application
- Nested `/guide/folder/subfolder/index.md` becomes `/guide/folder/subfolder`
- Other files become `/guide/folder/file` 

Example:

```
guide/halo/index.md           → /guide/halo
guide/halo/haloreach/index.md → /guide/halo/haloreach
guide/halo/haloreach/levels.md → /guide/halo/haloreach/levels
```

## Philosophy

Content is intentionally simple:

- No database
- No CMS
- No hidden admin system

If something is wrong, open a PR.
