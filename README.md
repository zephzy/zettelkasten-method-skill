# Zettelkasten Method Skill

Turn AI reading into reusable Zettelkasten knowledge assets.

Distill the Zettelkasten method into an executable AI workflow.

把 AI 阅读变成可复用的卡片笔记知识资产。

> Not another summarizer. This prompt pack helps AI agents convert raw material into traceable cards, meaningful links, bottom-up outlines, drafts, and quality reports.

## What It Does

Most AI tools summarize material. This prompt pack does something different:

1. Break raw material into fleeting notes.
2. Rewrite source ideas into literature notes with traceable sources.
3. Transform them into atomic permanent notes in your own words.
4. Propose meaningful links between notes.
5. Build a bottom-up outline from connected notes.
6. Draft an article while preserving note provenance.
7. Run a quality check against Zettelkasten principles.

中文说明：它不是“让 AI 帮你总结文章”，而是让 AI 按卡片笔记法的流程，把素材转化为可积累、可链接、可复用的知识资产。

## Two-minute Demo

The demo uses the official OpenAI Prompting guide as a public AI-learning source:

- Source snapshot: [`openai-prompting-guide-demo/source-snapshot.md`](templates-and-examples/examples/openai-prompting-guide-demo/source-snapshot.md)
- Ordinary summary baseline: [`openai-prompting-guide-demo/ordinary-summary.md`](templates-and-examples/examples/openai-prompting-guide-demo/ordinary-summary.md)
- Zettelkasten dry-run output: [`openai-prompting-guide-demo/dry-run-output.md`](templates-and-examples/examples/openai-prompting-guide-demo/dry-run-output.md)

What the dry run produces:

- 4 fleeting notes
- 3 literature notes with the official source URL
- 4 permanent notes in the user's own words
- 4 proposed links with relationship explanations
- 1 bottom-up topic outline
- 1 short draft
- 1 quality report

中文说明：这个 demo 展示同一份材料如何从“普通总结”升级为“可继续生长的知识卡片系统”。

## Who It Is For

- Students and researchers building a durable knowledge base.
- Writers and creators who want grounded, non-generic drafts.
- Obsidian / Markdown users who want AI-assisted note workflows.
- AI learning communities that need a repeatable learning-to-writing system.

## Quick Start

1. Open [`prompts/zettelkasten-method-skill.md`](prompts/zettelkasten-method-skill.md).
2. Copy the full prompt into your AI agent.
3. Paste one article, paper excerpt, transcript, or reading note.
4. Ask the agent to run the complete Zettelkasten workflow.

Example request:

```text
Use the Zettelkasten Method Skill on the source material below.
Output fleeting notes, literature notes, permanent notes, proposed links,
a topic outline, a short draft, and a quality report.

Source:
[paste material here]
```

中文用法：

```text
请使用 Zettelkasten Method Skill 处理下面的学习材料。
请输出闪念卡、文献卡、永久卡、关联链接、主题大纲、短文初稿和质量检查报告。
```

## Workflow

```text
Raw Material
  -> Fleeting Notes
  -> Literature Notes
  -> Permanent Notes
  -> Link Map
  -> Topic Outline
  -> Draft
  -> Quality Report
```

## Why This Is Not Just AI Summary

| Ordinary AI Summary | Zettelkasten Method Skill |
| --- | --- |
| Compresses the source | Converts source material into reusable notes |
| Produces one-off output | Builds a growing knowledge base |
| Often loses provenance | Keeps source fields and note IDs |
| Writes top-down | Synthesizes bottom-up from linked notes |
| Focuses on fluency | Checks atomicity, traceability, and link quality |

## Included Files

- [`prompts/zettelkasten-method-skill.md`](prompts/zettelkasten-method-skill.md): the core prompt pack.
- [`templates-and-examples/templates/`](templates-and-examples/templates): reusable Markdown templates.
- [`templates-and-examples/examples/source-ai-learning-excerpt.md`](templates-and-examples/examples/source-ai-learning-excerpt.md): sample source material.
- [`templates-and-examples/examples/ai-learning-mini-kb/dry-run-output.md`](templates-and-examples/examples/ai-learning-mini-kb/dry-run-output.md): complete manual dry-run output.
- [`templates-and-examples/examples/openai-prompting-guide-demo/dry-run-output.md`](templates-and-examples/examples/openai-prompting-guide-demo/dry-run-output.md): second public-source demo.
- [`templates-and-examples/examples/before-after-demo.md`](templates-and-examples/examples/before-after-demo.md): summary-vs-method demo.

## v0.1 Acceptance Criteria

- Generates at least 3 fleeting notes.
- Generates at least 2 literature notes with source fields.
- Generates at least 2 permanent notes in the user's own words.
- Proposes at least 3 links with relationship explanations.
- Builds one topic outline.
- Drafts one short article.
- Produces one quality report.

## Roadmap

- v0.1: prompt pack, templates, example knowledge base, dry-run demo.
- v0.2: optional card-quality checker script.
- v0.3: Obsidian vault starter kit.
- v0.4: Claude Code / Codex skill packaging variants.

## License

MIT
