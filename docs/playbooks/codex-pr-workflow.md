# Codex Pull Request Workflow

When making changes to the AugMind Ops repository, Codex must follow this standard workflow.

## 1) Branch Naming Rules

Create a new branch for each task using one of these patterns:

- `content/<topic>`
- `setup/<feature>`
- `fix/<issue>`

Examples:

- `content/langchain-explainer`
- `content/vector-database-explainer`
- `setup/mkdocs-blog-plugin`
- `fix/navigation-indentation`

## 2) Scope of Changes

- Make changes only related to the specific task.
- Avoid mixing unrelated fixes or refactors in the same branch.
- Keep updates aligned with repository structure and templates.

## 3) Validation Checklist

Before opening a pull request, run and verify:

- `mkdocs build`
- Navigation links are valid and resolve correctly

## 4) Pull Request Requirements

Use this title format:

```text
<category>: <short description>
```

Examples:

- `content: add langchain explainer`
- `setup: add mkdocs blog plugin`
- `fix: correct navigation indentation`

PR description must include:

- Summary
- What was added or changed
- Files modified
- Testing notes

## 5) Reusable Prompt Pattern

When requesting Codex updates, use this structure:

```text
Follow the Codex PR workflow.

Task:
<Create concise task statement>

Steps:
1. Create branch <category/topic>
2. Make only task-related changes
3. Update navigation or docs structure if needed
4. Ensure MkDocs build succeeds
5. Create a pull request using the repository PR template
```

Example:

```text
Follow the Codex PR workflow.

Task:
Create a new explainer article for "What is LangChain".

Steps:
1. Create branch content/langchain-explainer
2. Add article in docs/explainers/
3. Update navigation if needed
4. Ensure MkDocs build succeeds
5. Create a pull request using the repository PR template
```

## 6) Commit Message Convention

Use clear, category-based commit messages:

- `content: new article`
- `setup: configuration change`
- `fix: bug fix`
- `docs: documentation update`

Examples:

- `content: add langchain explainer`
- `setup: enable mkdocs blog plugin`
- `fix: correct mkdocs navigation`

## 7) Why This Workflow Works

Without a consistent workflow, AI-generated changes can be difficult to review and maintain. This process enforces:

1. Task-focused branches
2. Structured pull requests
3. Predictable validation before review

Flow:

```text
AI task -> feature branch -> structured PR -> review -> merge
```

This keeps the repository clean, readable, and maintainable over time.
