# Setting up Tags

Official docs: https://squidfunk.github.io/mkdocs-material/setup/setting-up-tags/

Why
- Tags help readers discover related content across pages (useful for blogs, playbooks, and explainers).

Simple approach (manual)
- Add a `tags` front matter field to posts/pages and manually maintain a `tags/index.md` that links to pages by tag.

Example front matter for a post/page:

```yaml
---
title: Example Post
tags:
  - agents
  - playbooks
---
```

Example `docs/tags/index.md` (manual tag index)

```markdown
# Tags

## agents
- [Post A](../blog/2026-03-01-first-post.md)

## playbooks
- [Codex Agent Task Playbook](../playbooks/codex-agent-tasks.md)
```

Automated tag pages
- For automatic tag indexes, use a blog/tagging plugin (search for `mkdocs` tag plugins). If you'd like, I can add one and generate tag pages automatically from front matter.

Notes
- The manual approach is low-dependency and easy to control.
- If you plan to publish many posts, automated tag pages are worth adding.
