# AugMind Ops

AugMind Ops is a personal **Augmented Mind Operating System** — a knowledgebase where human curiosity and AI collaboration transform complex technology into structured knowledge and actionable insights.

The project captures learning about software systems, AI tools, developer ecosystems, and enterprise products, then converts that knowledge into clear explanations, analysis, and operational playbooks.

## Project vision

Modern professionals interact with overwhelming amounts of technical information. AugMind Ops is designed as a human + AI knowledge engine that:

- captures ideas and learning
- explains complex technologies in simple terms
- analyzes enterprise software ecosystems
- summarizes community discussions and trends
- converts knowledge into actionable playbooks

This repository powers a static knowledge portal built with a JAMstack documentation approach.

## Key principles

1. **Augmented Intelligence**  
   Human reasoning enhanced with AI tools.
2. **Knowledge Structuring**  
   Information organized into searchable and structured documentation.
3. **Clarity**  
   Complex technology explained in simple language.
4. **Actionability**  
   Insights should lead to practical understanding or decisions.

## Knowledge categories

### Learn
Core technical concepts explained clearly.

Examples: APIs, Kubernetes, Databases, Networking

### Explainers
Technology explained in layman terms.

Examples: What is LangChain, What is an API Gateway, What is Vector Search

### Enterprise Intelligence
Analysis of enterprise software products.

Examples: Stripe platform overview, Databricks ecosystem, Snowflake architecture, BMC product portfolio

### Community Insights
Summaries of technical discussions from developer communities.

Possible sources: GitHub Discussions, Reddit developer forums, Hacker News, product community forums

### Playbooks
Practical guides for using tools and technologies.

Examples: Using Playwright for API testing, Setting up documentation portals, AI-assisted documentation workflows

## Tech stack

- **Documentation engine:** MkDocs
- **Theme:** Material for MkDocs
- **Hosting:** Vercel
- **Version control:** GitHub
- **AI assistance:** OpenAI Codex agents, Anthropic Claude models
- **Content format:** Markdown

## Repository structure

```text
augmind-ops/
├── docs/
│   ├── index.md
│   ├── learn/
│   ├── explainers/
│   ├── enterprise/
│   ├── community/
│   ├── playbooks/
│   └── glossary/
├── mkdocs.yml
├── requirements.txt
└── README.md
```

## Requirements

- Python 3.10+

Install dependencies:

```bash
pip install -r requirements.txt
```

Run locally:

```bash
mkdocs serve
```

Build static site:

```bash
mkdocs build
```

## Additional context for agents

For a richer, codex-oriented project brief, see [`PROJECT_CONTEXT.md`](PROJECT_CONTEXT.md).
