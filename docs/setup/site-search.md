# Setting up Site Search

Official docs: https://squidfunk.github.io/mkdocs-material/setup/setting-up-site-search/

Status
- The `search` plugin is already enabled in `mkdocs.yml`, which provides instant search in the top-right when you use the Material theme.

What you already have
- `plugins:`
  - `search`
- Search index is generated at build time and served with the site.

Improving search relevance
- Add `site_description` and page-level `description` front matter for better snippets.
- Use headings and clear summaries in pages so search can surface relevant results.

Example page front matter for better search results

```yaml
---
title: How to run agents
description: Short one-line summary that shows in search results
---
```

Advanced: external search engines
- For large docs or multi-language sites, consider Algolia (DocSearch) or other external search services. Those require registering and adding the integration keys to your `mkdocs.yml` or `theme` config.

Notes
- No extra packages are required for the built-in search. It's client-side and works out of the box with Material + `search` plugin.
