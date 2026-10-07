# GLOBAL-RULES.md

Behavioral guidelines to reduce common LLM coding mistakes. Merge with project-specific instructions as needed.

**Tradeoff:** These guidelines bias toward caution over speed. For trivial tasks, use judgment.

## 1. Think Before Coding

**Don't assume. Don't hide confusion. Surface tradeoffs.**

Before implementing:
- State your assumptions explicitly. If uncertain, ask.
- If multiple interpretations exist, present them - don't pick silently.
- If a simpler approach exists, say so. Push back when warranted.
- If something is unclear, stop. Name what's confusing. Ask.

## 2. Simplicity First

**Minimum code that solves the problem. Nothing speculative.**

- No features beyond what was asked.
- No abstractions for single-use code.
- No "flexibility" or "configurability" that wasn't requested.
- No error handling for impossible scenarios.
- If you write 200 lines and it could be 50, rewrite it.

Ask yourself: "Would a senior engineer say this is overcomplicated?" If yes, simplify.


## 2.1. Fewer Agents First

Prefer the smallest agent configuration that can safely complete the task.

- Do not activate a multi-agent workflow when a single agent with tools is sufficient.
- Add specialist agents only when they reduce real uncertainty, risk, or rework.
- If you activate multiple agents, state:
  - why each one is needed;
  - what success criterion each one owns;
  - what stops the loop.
- Multi-agent is not a default virtue. It must earn its complexity.


## 3. Surgical Changes

**Touch only what you must. Clean up only your own mess.**

When editing existing code:
- Don't "improve" adjacent code, comments, or formatting.
- Don't refactor things that aren't broken.
- Match existing style, even if you'd do it differently.
- If you notice unrelated dead code, mention it - don't delete it.

When your changes create orphans:
- Remove imports/variables/functions that YOUR changes made unused.
- Don't remove pre-existing dead code unless asked.

The test: Every changed line should trace directly to the user's request.

## 4. Goal-Driven Execution

**Define success criteria. Loop until verified.**

Transform tasks into verifiable goals:
- "Add validation" → "Write tests for invalid inputs, then make them pass"
- "Fix the bug" → "Write a test that reproduces it, then make it pass"
- "Refactor X" → "Ensure tests pass before and after"

For multi-step tasks, state a brief plan:
```
1. [Step] → verify: [check]
2. [Step] → verify: [check]
3. [Step] → verify: [check]
```

Strong success criteria let you loop independently. Weak criteria ("make it work") require constant clarification.

## 4.1. Agent Accountability

In multi-agent execution:

- every agent must have a bounded role;
- every handoff must have a reason;
- every loop must have a stop condition;
- every approval or rejection must be attributable;
- every persistent change must have an owner.

If no one owns the check, the check does not exist.


## 5. Memory Discipline

- Do not promote temporary reasoning, local fixes, session history, or draft conclusions to persistent memory by default.
- Treat validated project files as the source of truth.
- If retrieved memory conflicts with a canonical file, trust the canonical file.
- Retrieval is support, not authority.

---

**These guidelines are working if:** fewer unnecessary changes in diffs, fewer rewrites due to overcomplication, and clarifying questions come before implementation rather than after mistakes.