---
name: carryover
description: Prepare a copy-ready context handoff for continuing work in a new agent session.
disable-model-invocation: true
---

# Carryover

Create a context handoff that the user can paste into a new agent session to continue the current work.

Optimize for continuity, not conversation history.

## Process

1. **Review** the conversation and relevant available context. Identify the current goal and intended direction.
2. **Reconcile** decisions and progress. Prioritize the latest confirmed decisions over superseded ideas. Preserve important reasoning, constraints, and failed attempts.
3. **Select** information the next agent needs to continue effectively. If arguments are provided, prioritize that focus while retaining necessary dependencies.
4. **Compose** a self-contained Markdown handoff, organized around the actual work rather than a fixed template.
5. **Verify** that the next agent can understand the current state and identify what to do next without access to the previous conversation.

## Content

Include relevant information such as:

- **Goal:** What we're trying to achieve, preferably in 1–2 sentences.
- **Context:** Essential background, requirements, constraints, and decisions.
- **Progress:** What has been completed, attempted, or ruled out.
- **References:** Relevant files, paths, URLs, commits, and other artifacts.
- **Current state:** What's in progress, unresolved, or blocked.
- **Next steps:** Concrete actions needed to continue.

Adapt the structure to the task. Combine, rename, or omit sections as appropriate.

Preserve exact technical details when they affect continuation. Distinguish confirmed facts from assumptions and open questions.

Reference existing artifacts instead of duplicating them. Include essential context when those artifacts may be unavailable in the next session.

## Output

Return a single, copy-ready Markdown document directly in the conversation.

- Start with the main objective and end with the immediate next action when applicable.
- Keep the handoff concise without sacrificing essential context.
- Exclude irrelevant history, repetition, and superseded details.
- Redact credentials, secrets, and sensitive personal information.
- Preserve only verified decisions and progress; identify uncertainties.
- Include no commentary outside the handoff.
- Create files only when explicitly requested.
