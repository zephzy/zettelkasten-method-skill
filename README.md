# Zettelkasten Method Skill

Turn AI reading into reusable Zettelkasten knowledge assets.

把 AI 阅读变成可积累、可链接、可复用的卡片笔记知识资产。

This repository packages the Zettelkasten method as an Agent Skills-style workflow. It helps AI agents transform source material into fleeting notes, literature notes, permanent notes, meaningful links, bottom-up outlines, drafts, and quality reports.

它不是“总结器提示词”，而是把卡片笔记法里的专家流程拆成可执行步骤，让 AI 帮你建立能继续生长的知识系统。

## Why It Exists

Most AI reading workflows stop at a polished summary. This skill is designed for people who want durable knowledge assets: notes that preserve sources, express ideas in your own words, link to other ideas, and become grounded drafts.

大多数 AI 阅读只产出一次性答案。这个 skill 更关注长期积累：来源可追溯、观点可拆分、卡片可链接，最后的文章能从卡片网络里长出来。

| Ordinary AI Summary | Zettelkasten Method Skill |
| --- | --- |
| Compresses the source | Converts material into reusable notes |
| Produces one-off output | Builds a growing knowledge base |
| Often loses provenance | Keeps source fields and note IDs |
| Writes top-down | Synthesizes bottom-up from linked notes |
| Optimizes for fluency | Checks atomicity, traceability, and link quality |

## Quick Start

### Agent Skills-compatible tools

Copy the skill folder into your agent's skills directory:

```text
skills/zettelkasten-method/
```

Then ask your agent:

```text
Use the Zettelkasten Method Skill on the source material below.
Return fleeting notes, literature notes, permanent notes, proposed links,
a topic outline, a short draft, and a quality report.

Source:
[paste material here]
```

如果你的工具支持 `SKILL.md` 风格的 skill 文件夹，优先使用这个方式。这样 agent 会把它当成一个可复用工作流，而不是一段临时提示词。

### Any AI agent

If your agent does not support skill folders, use the portable prompt:

```text
prompts/zettelkasten-method-skill.md
```

Paste the full prompt into ChatGPT, Claude, Codex, Cursor, or another capable agent, then provide your source material.

如果平台暂时不支持安装 skill，就直接复制 portable prompt。输出结构和质量标准仍然与正式 skill 保持一致。

### Try the demo

Open the public-source dry run:

- [Source snapshot](templates-and-examples/examples/openai-prompting-guide-demo/source-snapshot.md)
- [Ordinary summary baseline](templates-and-examples/examples/openai-prompting-guide-demo/ordinary-summary.md)
- [Zettelkasten dry-run output](templates-and-examples/examples/openai-prompting-guide-demo/dry-run-output.md)

这个 demo 使用 OpenAI 官方 Prompting guide 的公开材料，展示同一份内容如何从普通总结变成可追溯、可链接、可复用的知识卡片。

## What the Skill Produces

```text
Raw Material
  -> Source Snapshot
  -> Fleeting Notes
  -> Literature Notes
  -> Permanent Notes
  -> Proposed Links
  -> Topic Outline
  -> Short Draft
  -> Quality Report
```

The output is intentionally inspectable. Every literature note keeps source information, every permanent note is atomic, every link explains a relationship, and every draft claim should trace back to note IDs.

输出不是为了“看起来很会写”，而是为了能检查、能复盘、能继续扩展。卡片、链接和初稿之间应该有清楚的证据链。

## Repository Structure

```text
.
+-- skills/
|   +-- zettelkasten-method/
|       +-- SKILL.md
+-- prompts/
|   +-- zettelkasten-method-skill.md
+-- templates-and-examples/
|   +-- templates/
|   +-- examples/
+-- PROJECT_CARD.md
+-- LICENSE
+-- README.md
```

- [`skills/zettelkasten-method/SKILL.md`](skills/zettelkasten-method/SKILL.md): canonical Agent Skills-style entrypoint.
- [`prompts/zettelkasten-method-skill.md`](prompts/zettelkasten-method-skill.md): portable prompt for agents that cannot install skills.
- [`templates-and-examples/templates/`](templates-and-examples/templates): reusable Markdown templates.
- [`templates-and-examples/examples/`](templates-and-examples/examples): source material, before/after comparison, and dry-run outputs.

## Skill Anatomy

The canonical skill follows the common Agent Skills pattern:

- YAML frontmatter with `name` and `description`.
- An overview that defines the skill's purpose.
- Input expectations and fallback behavior.
- A fixed workflow from source snapshot to quality report.
- Output contracts with stable note IDs.
- Quality rules and failure modes.

这种结构的好处是：别人打开仓库后能立刻看懂它是一个真正的 workflow skill，而不是散装提示词。

## Example Invocation

```text
Use the Zettelkasten Method Skill on this article excerpt.

Goal:
- Build reusable notes for future AI-learning writing.

Language:
- Bilingual

Source metadata:
- Title: [title]
- URL: [url]

Source:
[paste excerpt]
```

Expected sections:

- `Source Snapshot`
- `Fleeting Notes`
- `Literature Notes`
- `Permanent Notes`
- `Proposed Links`
- `Topic Outline`
- `Short Draft`
- `Quality Report`
- `Next Actions`

## Demo Result

The OpenAI Prompting Guide demo produces:

- 4 fleeting notes
- 3 literature notes with the official source URL
- 4 permanent notes in the user's own words
- 4 proposed links with relationship explanations
- 1 bottom-up topic outline
- 1 short draft
- 1 quality report

它证明这个项目的重点不是“把文章压缩短一点”，而是把材料变成可以继续组织、连接和写作的知识资产。

## Good For

- students and researchers building a durable knowledge base
- Obsidian or Markdown users who want AI-assisted note workflows
- writers who need grounded drafts from accumulated notes
- AI-learning communities that want repeatable reading-to-writing workflows

## Roadmap

- v0.1: Agent Skills-style workflow, portable prompt, templates, and demos.
- v0.2: optional card-quality checker script.
- v0.3: Obsidian vault starter kit.
- v0.4: lightweight eval cases for output quality regression.

## License

MIT
