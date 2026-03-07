# Footnotes

Official docs: https://squidfunk.github.io/mkdocs-material/reference/footnotes/

How to use

MkDocs + Material supports footnotes via the Markdown `footnotes` extension. Once enabled you can create footnotes inline like this:

Example:

```markdown
Here is a sentence with a footnote.[^1]

[^1]: This is the footnote text — it will appear at the bottom of the page.
```

What I enabled for you
- `pymdownx.extra` — provides a set of helpful Markdown enhancements.
- `markdown.extensions.footnotes` — enables footnote syntax.

Notes
- No extra Python packages are required beyond `pymdown-extensions`, which is already installed in the project's venv.
- If you want numbered footnote markers or a different style, we can add small CSS overrides to tweak the appearance.
