# Site Analytics

Official docs: https://squidfunk.github.io/mkdocs-material/setup/setting-up-site-analytics/

Options
- Google Analytics (gtag) — recommended for general analytics.
- Plausible, Fathom, or other privacy-focused analytics — usually added via `extra` or template snippets.

Google Analytics (gtag) example (add to `mkdocs.yml`):

```yaml
theme:
  name: material
  # ... other theme settings

extra:
  analytics:
    provider: gtag
    gtag:
      - 'G-XXXXXXXXXX'  # replace with your Measurement ID
```

Classic Google Analytics (older) example (less recommended):

```yaml
google_analytics:
  - 'UA-XXXXX-Y'
  - auto
```

Notes
- Replace the Measurement ID with your real ID from Google Analytics / Google Tag Manager.
- Some hosting platforms (Vercel, Netlify) also offer built-in analytics integrations.
- If you prefer a privacy-first provider (Plausible, Fathom), I can add the snippet and show how to inject it into the site using `extra_javascript` or a small template override.
