## Guardrails

- **NEVER modify AGENTS.md without approval** — Read-only for the agent
- **NEVER make irreversible changes without approval**
- **NEVER commit unless explicitly asked**

## Working Philosophy

- **Research before code** — Explore codebase and docs first
- **Propose, don't execute** — Present plan, wait for approval
- **Chunk-based delivery** — Complete small pieces, checkpoint
- **Fix root causes** — No workarounds unless stuck
- **Say it when the architecture is tangled** — Don't quietly ship into a mess
- **Concrete plans before big changes** — Target structure, what gets deleted, migration sequence

## Code Principles

- **Readability over cleverness** — Every concept gets one obvious home
- **KISS first** — No layers, registries, or abstractions unless they clearly reduce complexity
- **Human co-ownership is required** — If only the AI can navigate the code, the architecture is wrong
- **Delete dead code aggressively** — No compatibility shims for things nothing uses
- **Glass-box, not black-box** — Memory, reasoning, prompts, diagnostics all visible

## Architecture Principles

- **One source of truth per kind of state** — Never let stores silently compete
- **Separate deterministic logic from LLM logic** — Code owns routing/scheduling/gates; LLM owns synthesis/interpretation
- **One obvious entry point per feature** — If you can't quickly answer "where does this live?", reorganize
- **Preserve what's differentiated** — Don't simplify by flattening the product into something generic

## Verification

- Run tests after code changes
