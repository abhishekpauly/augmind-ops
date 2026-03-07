# Social Cards

Official docs: https://squidfunk.github.io/mkdocs-material/setup/setting-up-social-cards/

Why
- Social cards (open graph / Twitter cards) make links to your site look good when shared on social platforms.

Quick steps
1. Add a default social image to `docs/assets/images/social-default.png` (or another path under `docs/`).
2. Add site metadata and theme config to `mkdocs.yml`.

Example snippet for `mkdocs.yml` (copy into your file and edit paths/values):

```yaml
site_name: AugMind Ops
site_description: Augmented Mind Operating System for structured technical knowledge
site_url: https://augmind-ops.vercel.app

extra:
  social:
    - type: twitter
      image: assets/images/social-default.png
      description: "AugMind Ops — structured technical knowledge"

# Theme block (keep existing theme config)
theme:
  name: material
  features:
    - navigation.tabs
    - navigation.sections
```

Page-specific cards
- You can add page-level metadata in the top of any Markdown file. Example front matter:

```yaml
---
title: Example Page
description: Short description for social preview
image: assets/images/social-example.png
---
```

Notes
- Create images at recommended sizes (1200×630px for OG, 1200×675 sometimes used). Adjust filenames in the examples above.
- See the official guide for advanced options and automatic generation.
