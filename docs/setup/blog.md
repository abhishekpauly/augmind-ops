# Setting up a Blog

Official docs: https://squidfunk.github.io/mkdocs-material/setup/setting-up-a-blog/

Why
- Add a blog section for announcements, changelogs, or articles.

Simple pattern (no extra plugins)
- Create a `docs/blog/index.md` that lists posts and links to `docs/blog/<post>.md` pages.
- Add `Blog` to your `nav` in `mkdocs.yml`.

Example `nav` entry (in `mkdocs.yml`):

```yaml
nav:
  - Blog:
      - Overview: blog/index.md
      - Post 1: blog/2026-03-01-first-post.md
```

Example `docs/blog/index.md` (simple list)

```markdown
# Blog

- [First post](2026-03-01-first-post.md) — 2026-03-01
- [Another post](2026-02-10-another-post.md) — 2026-02-10
```

Using plugins for a richer blog
- There are community plugins (e.g., mkdocs-blog-plugin) that can provide automatic indices, pagination, and tags. If you want that, we can add the plugin to `requirements.txt` and enable it in `mkdocs.yml`.

Notes
- The simple approach keeps everything under version control and works with Material's features like social cards and search.
- If you want automatic feeds (Atom/RSS) or tag pages, tell me and I will wire a plugin in and create sample posts.
