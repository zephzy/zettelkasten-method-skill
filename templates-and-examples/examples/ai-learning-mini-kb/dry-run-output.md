# Dry Run Output: AI Learning Mini Knowledge Base

This dry run uses `examples/source-ai-learning-excerpt.md`.

## 1. Source Snapshot

- Source title: Why Active AI Learning Beats Passive Prompt Copying
- Source type: short learning article excerpt
- Source author or origin: example source created for this repository
- Date: 2026-07-01
- URL or location: local example
- Main theme: AI learning becomes deeper when users turn model interaction into a feedback loop and preserve reusable learning artifacts.

## 2. Fleeting Notes

### F-001
- Capture: Copying prompts can feel productive while producing shallow learning.
- Why it caught attention: It describes a common false sense of progress.
- Possible direction: Compare output consumption with knowledge construction.

### F-002
- Capture: The important step is the loop: ask, test, revise, and apply.
- Why it caught attention: This sounds like the core mechanism of active AI learning.
- Possible direction: Turn this loop into a reusable study workflow.

### F-003
- Capture: Saved artifacts convert chat history into a personal knowledge base.
- Why it caught attention: This connects AI learning with durable note systems.
- Possible direction: Use Zettelkasten cards as the artifact layer.

### F-004
- Capture: Strong learners use AI to diagnose misconceptions, not just summarize.
- Why it caught attention: It reframes AI as a feedback system.
- Possible direction: Design prompts that expose blind spots.

## 3. Literature Notes

### L-001
- Source: Why Active AI Learning Beats Passive Prompt Copying
- Location: paragraph 1
- Source claim: Beginners often use AI tools as answer machines, which can feel productive but lead to shallow learning.
- Rewritten explanation: Passive AI use creates the appearance of progress because it quickly produces answers, but it does not necessarily help the learner build reusable understanding.
- Useful for: explaining why prompt copying is a weak learning strategy.

### L-002
- Source: Why Active AI Learning Beats Passive Prompt Copying
- Location: paragraph 2
- Source claim: AI becomes more useful when the learner asks, tests, revises, and applies.
- Rewritten explanation: The value of AI in learning comes from iterative feedback, not from the first generated answer.
- Useful for: defining active AI learning as a loop.

### L-003
- Source: Why Active AI Learning Beats Passive Prompt Copying
- Location: paragraph 3
- Source claim: Learners should preserve questions, mistakes, explanations, examples, and follow-up tasks as artifacts.
- Rewritten explanation: Learning improves when AI conversations leave reusable traces that can be reviewed, linked, and expanded later.
- Useful for: connecting AI usage with knowledge management.

### L-004
- Source: Why Active AI Learning Beats Passive Prompt Copying
- Location: paragraph 4
- Source claim: Strong learners use AI to compare concepts, diagnose misconceptions, and turn curiosity into experiments.
- Rewritten explanation: Advanced AI learning uses the model as a tool for testing and refining thinking, not just for producing summaries.
- Useful for: distinguishing shallow AI use from feedback-driven learning.

## 4. Permanent Notes

### P-001 - Passive AI use can hide shallow learning
- Claim: Fast AI answers can make learning feel efficient even when understanding remains weak.
- Explanation: If a learner only copies prompts and accepts outputs, the activity produces visible text but may not create a reusable mental model.
- Example: A student who asks for a summary of backpropagation may recognize the words later but fail to explain why gradients are propagated backward.
- Source basis: L-001
- Possible links: P-002, P-004

### P-002 - Active AI learning depends on a feedback loop
- Claim: AI supports deeper learning when interaction becomes a loop of asking, testing, revising, and applying.
- Explanation: The first answer is only a starting point. Understanding grows when the learner challenges the answer, checks gaps, and uses the result in a task.
- Example: After receiving an explanation of attention mechanisms, the learner asks for counterexamples, solves a toy problem, and revises their explanation.
- Source basis: L-002
- Possible links: P-001, P-003, P-004

### P-003 - Learning artifacts turn chats into a knowledge base
- Claim: AI conversations become more valuable when they leave durable artifacts.
- Explanation: Questions, mistakes, corrected explanations, examples, and follow-up tasks can be saved as reusable notes instead of disappearing in chat history.
- Example: A learner can convert a mistaken explanation into a permanent note titled "Attention is not the same as explanation."
- Source basis: L-003
- Possible links: P-002, P-004

### P-004 - Good AI prompts expose blind spots
- Claim: A strong learning prompt should reveal what the learner does not yet understand.
- Explanation: Asking for summaries confirms surface familiarity, while asking for tests, comparisons, and misconception diagnosis creates feedback.
- Example: Instead of asking "Summarize transformers," ask "Give me three misconceptions about transformers and test whether my explanation contains them."
- Source basis: L-004
- Possible links: P-001, P-002, P-003

## 5. Proposed Links

- `P-001` -> `P-002`
  - Relationship: problem to remedy.
  - Why this link matters: P-001 explains why passive AI use fails; P-002 explains the workflow that repairs the failure.

- `P-002` -> `P-003`
  - Relationship: process to infrastructure.
  - Why this link matters: The feedback loop needs saved artifacts to become cumulative rather than temporary.

- `P-004` -> `P-002`
  - Relationship: quality mechanism inside the loop.
  - Why this link matters: Blind-spot prompts make the ask-test-revise-apply loop more rigorous.

- `P-003` -> existing note `[[Zettelkasten as learning infrastructure]]`
  - Relationship: application.
  - Why this link matters: Durable AI learning artifacts can be implemented as Zettelkasten cards.

## 6. Topic Outline

## Working Title

AI Learning Works Best When It Becomes a Feedback Loop

## Thesis

AI tools become effective learning partners when learners stop treating them as answer machines and instead use them to test understanding, preserve artifacts, and build reusable knowledge.

## Outline

1. Passive AI use creates a false sense of progress
   - Supported by: P-001
   - Point: Fast answers can produce text without producing understanding.

2. The core upgrade is a feedback loop
   - Supported by: P-002, P-004
   - Point: Ask-test-revise-apply turns AI output into active learning.

3. Learning must leave artifacts
   - Supported by: P-003
   - Point: Notes, mistakes, examples, and tasks make learning cumulative.

4. Zettelkasten can serve as the artifact layer
   - Supported by: P-003 and proposed link to `[[Zettelkasten as learning infrastructure]]`
   - Point: Card-based notes make AI learning traceable and reusable.

## 7. Short Draft

# AI Learning Works Best When It Becomes a Feedback Loop

Many learners use AI tools in a way that feels productive but stays shallow. They copy a prompt, receive a fluent answer, and move on. The problem is that visible output is not the same as understanding. A summary can make a concept feel familiar while leaving the learner unable to explain or apply it later (P-001).

A better pattern is to treat AI interaction as a feedback loop. The first answer should not be the final product. It should become the beginning of a cycle: ask a question, test the answer, revise the explanation, and apply the idea in a small task. This loop forces the learner to turn passive reading into active thinking (P-002).

The quality of the loop depends on the prompts used inside it. A weak prompt asks only for a summary. A stronger prompt asks the model to expose blind spots: compare similar concepts, generate test questions, diagnose misconceptions, or challenge the learner's explanation. These prompts make misunderstanding visible (P-004).

The final step is to preserve learning artifacts. Questions, mistakes, corrected explanations, examples, and follow-up tasks should not disappear inside chat history. They can become durable notes that support future review and writing (P-003). This is where a Zettelkasten workflow becomes useful: it turns AI-assisted learning into a growing knowledge system instead of a sequence of disposable conversations.

## 8. Quality Report

- Atomicity: pass. Each permanent note has one central claim.
- Own-words rewriting: pass. Literature and permanent notes restate ideas without long copying.
- Source traceability: pass. Literature notes include source and location fields.
- Link quality: pass. Links explain problem/remedy, process/infrastructure, and quality mechanism relationships.
- Bottom-up synthesis: pass. The outline and draft are built from permanent note IDs.
- Unsupported claims: none obvious. The Zettelkasten application is framed as an implementation suggestion, not a source claim.
- Notes to split or merge: none for v0.1. P-003 could later split into "artifact preservation" and "knowledge base infrastructure" if expanded.

## 9. Next Actions

- Improve the notes: add one real example from the user's own AI study session.
- Connect to an existing knowledge base: link P-003 to notes about Obsidian, spaced repetition, or learning logs.
- Expand into writing: turn the draft into a longer article comparing "AI as answer machine" vs "AI as feedback system."
