# Dry Run Output: OpenAI Prompting Guide Demo

This demo uses `source-snapshot.md`, which points to the official OpenAI Prompting guide:

https://developers.openai.com/api/docs/guides/prompting

## 1. Source Snapshot

- Source title: Prompting guide
- Source type: official technical guide
- Source author or origin: OpenAI developer documentation
- Date: unknown
- URL or location: https://developers.openai.com/api/docs/guides/prompting
- Main theme: Prompting is an iterative engineering practice where instructions, evaluation, and versioning shape reliable model behavior.

## 2. Fleeting Notes

### F-001
- Capture: Prompting is not just wording; it is a way to control behavior.
- Why it caught attention: It reframes prompts as part of the system design.
- Possible direction: Explain why prompt packs need quality gates.

### F-002
- Capture: Prompt improvement depends on testing, not guessing.
- Why it caught attention: This makes prompt design feel closer to software engineering.
- Possible direction: Link prompt iteration to evaluation loops.

### F-003
- Capture: Production prompts should be versioned like code.
- Why it caught attention: It gives prompt work a maintainability frame.
- Possible direction: Argue that prompt workflows need reusable artifacts.

### F-004
- Capture: Better prompts reduce ambiguity for both model and user.
- Why it caught attention: It connects instruction clarity with output reliability.
- Possible direction: Build a note about constraints as quality infrastructure.

## 3. Literature Notes

### L-001
- Source: OpenAI Prompting guide
- Location: https://developers.openai.com/api/docs/guides/prompting
- Source claim: Prompt quality strongly influences the usefulness and reliability of model output.
- Rewritten explanation: The way a task is framed affects whether the model gives vague, generic, or useful responses.
- Useful for: explaining why prompt design deserves systematic attention.

### L-002
- Source: OpenAI Prompting guide
- Location: https://developers.openai.com/api/docs/guides/prompting
- Source claim: Prompting benefits from iteration, testing, and evaluation.
- Rewritten explanation: Effective prompt work is not a one-shot activity; it improves through cycles of trying, observing failures, and revising.
- Useful for: connecting prompt writing to engineering feedback loops.

### L-003
- Source: OpenAI Prompting guide
- Location: https://developers.openai.com/api/docs/guides/prompting
- Source claim: Production prompt work should be managed with care, including version control and systematic improvement.
- Rewritten explanation: Prompts become maintainable when treated as evolving project assets rather than disposable chat messages.
- Useful for: explaining why a prompt pack can be a real developer artifact.

## 4. Permanent Notes

### P-001 - Prompt design is behavior design
- Claim: A prompt is not just text; it is a lightweight behavior specification for an AI system.
- Explanation: Instructions, constraints, examples, and output contracts shape what the model pays attention to and how it responds.
- Example: Asking for "notes" produces a loose list, while asking for fleeting notes, literature notes, permanent notes, links, and a quality report produces a structured knowledge workflow.
- Source basis: L-001
- Possible links: P-002, P-004

### P-002 - Prompt quality improves through feedback loops
- Claim: Good prompts are discovered through testing and revision, not written perfectly on the first attempt.
- Explanation: A prompt becomes reliable when failures are observed, categorized, and converted into clearer instructions or quality checks.
- Example: If generated permanent notes contain two ideas, the next prompt revision should add an atomicity rule and a split-note repair step.
- Source basis: L-002
- Possible links: P-001, P-003

### P-003 - Prompts become assets when they are versioned
- Claim: A reusable prompt should be maintained like a project asset.
- Explanation: Once a prompt controls a repeatable workflow, it needs examples, changelog-like reasoning, versioned revisions, and tests against sample inputs.
- Example: This Zettelkasten prompt pack keeps templates and dry-run outputs so users can inspect expected behavior.
- Source basis: L-003
- Possible links: P-002, P-004

### P-004 - Output contracts make AI workflows inspectable
- Claim: Structured output sections turn vague AI assistance into a workflow that can be checked.
- Explanation: When the prompt requires fixed sections and quality criteria, users can see which part of the workflow succeeded or failed.
- Example: A Zettelkasten output with note IDs, source fields, link explanations, and a quality report is easier to audit than a smooth summary.
- Source basis: L-001, L-002
- Possible links: P-001, P-003

## 5. Proposed Links

- `P-001` -> `P-004`
  - Relationship: specification to inspection.
  - Why this link matters: If a prompt defines behavior, then an output contract makes that behavior visible and reviewable.

- `P-002` -> `P-003`
  - Relationship: iteration to maintainability.
  - Why this link matters: Feedback loops produce prompt improvements; versioning preserves those improvements over time.

- `P-003` -> `P-004`
  - Relationship: asset management to quality control.
  - Why this link matters: A maintained prompt pack needs output criteria so future changes can be judged.

- `P-001` -> existing note `[[Methodology distillation as prompt engineering]]`
  - Relationship: application.
  - Why this link matters: Distilling a method into a prompt means translating tacit workflow into explicit behavior instructions.

## 6. Topic Outline

## Working Title

Prompt Packs Should Be Treated Like Knowledge Workflow Software

## Thesis

Reusable prompts become valuable when they are treated as behavior specifications that can be tested, versioned, and audited through structured outputs.

## Outline

1. Prompt design is behavior design
   - Supported by: P-001
   - Point: Prompt wording shapes the model's task behavior.

2. Reliable prompts need feedback loops
   - Supported by: P-002
   - Point: Prompt quality improves by observing failures and revising instructions.

3. Prompt packs should be versioned assets
   - Supported by: P-003
   - Point: A reusable prompt needs examples and maintainable revisions.

4. Output contracts make prompt behavior auditable
   - Supported by: P-004
   - Point: Structured sections and quality checks reveal whether the workflow worked.

## 7. Short Draft

# Prompt Packs Should Be Treated Like Knowledge Workflow Software

A reusable prompt is more than a clever instruction. It is a lightweight behavior specification for an AI system. The prompt tells the model what role to take, what constraints to respect, what output shape to follow, and what quality bar to meet. In that sense, prompt design is behavior design (P-001).

This is why strong prompt packs should not be treated as one-off chat messages. They improve through feedback loops. A first version may produce useful output, but failures reveal where the workflow is under-specified. If permanent notes contain multiple ideas, the prompt needs a stronger atomicity rule. If links are only tags, the prompt needs relationship explanations. Reliable prompting grows through this cycle of test, observe, revise, and test again (P-002).

Once a prompt controls a repeatable workflow, it becomes a project asset. It needs examples, expected outputs, and a clear record of what good behavior looks like. Versioning matters because a prompt pack can regress just like code: a new instruction can make outputs longer, vaguer, or less traceable (P-003).

Structured output contracts make this process inspectable. A Zettelkasten prompt that requires source fields, note IDs, link explanations, and a quality report is easier to evaluate than a fluent summary. Users can see which stage succeeded and which stage needs repair (P-004). That is the difference between asking AI for an answer and building a reusable knowledge workflow.

## 8. Quality Report

- Atomicity: pass. Each permanent note has one central idea.
- Own-words rewriting: pass. The notes paraphrase the source snapshot and avoid long copying.
- Source traceability: pass. Literature notes include the official source URL.
- Link quality: pass. Links explain specification/inspection, iteration/maintenance, and asset/quality relationships.
- Bottom-up synthesis: pass. The outline and draft are built from permanent notes.
- Unsupported claims: none obvious. Claims about versioning and evaluation are framed as prompt-pack implications grounded in the source snapshot.
- Notes to split or merge: none for the demo. P-003 could later split into "versioning" and "expected outputs" if the article expands.

## 9. Next Actions

- Improve the notes: add a real failed prompt output and show which rule repairs it.
- Connect to an existing knowledge base: link P-002 to notes on test-driven development and learning feedback loops.
- Expand into writing: turn the draft into a README section explaining why this repository includes dry-run examples.
