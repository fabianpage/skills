# Agents

Includes an adapted `AGENTS.md` from [eeshansrivastava89/skills](https://github.com/eeshansrivastava89/skills/blob/main/skills/guardrails/agent-guardrails/SKILL.md).

# Skills

Adapted from [mattpocock/skills@5d78bd0](https://github.com/mattpocock/skills) — only the skills I currently use are included. The main adaptation is that issues are tracked in a local `/issues` folder instead of GitHub.


---

## Workflow

### `/grill-with-docs` — Align understanding

**Start here.** Run `/grill-with-docs "what do I want to achieve?"` to align the AI's and user's knowledge before doing any work.

- Clarified terms and concepts are written to `CONTEXT.md` to build a shared Ubiquitous Language.

---

### `/to-prd` — Create a Product Requirement Document

Run in the **same session** as `/grill-with-docs`.

- Produces a PRD that serves as input for the next step.

---

### `/to-issues` — Break down work into issues

Can be run in a **new session**.

- Creates an `/issues` folder with one file per step.
- Each issue should be reviewed for quality:
  - Can each step be tested individually?
  - Are the steps small, concrete, and solvable?

---

### `/implement issues/01_xxxxxx` — Implement an issue

Must be run in a **new, empty session**.

- Implements a single issue from the `/issues` folder.
