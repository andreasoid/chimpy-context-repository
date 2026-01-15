# Company Context Repository Blueprint

## Purpose
This repository is the **single source of truth** for how the company thinks, decides, and acts.

It exists to:
- Create shared context
- Enable fast, aligned decisions
- Reduce ambiguity and politics
- Serve as input for strategy, execution, onboarding, and AI systems

If something is not written here, it is **not a rule, not strategy, and not a commitment**.

---

## Core Principles

- **Clarity over completeness**
- **Short over exhaustive** (1–2 pages per document)
- **Written truth over tribal knowledge**
- **Decisions have owners** (see `governance.md`)
- **Review over authority**

---

## Repository Structure

```
/context
  constitution.md
  governance.md

  vision.md
  mission.md

  principles.md
  rules.md

  target_audience.md

  strategy_now.md
  strategy_next.md
  strategy_later.md

  roadmap.md

  prd_template.md
  prds/

  rfcs/
  archive/
```

Each document has **one clear owner**.

---

## Document Rules

All documents MUST:
- Be written in plain Markdown
- Fit on 1–2 pages
- Use bullet points where possible
- Describe what is **true**, not aspirational
- Avoid buzzwords and slogans

All documents MUST include this header:

```md
---
owner: <role or person>
status: draft | approved | deprecated
version: x.y
last_reviewed: YYYY-MM-DD
review_cycle: 3m | 6m | 12m
---
```

---

## Governance Alignment

Decision rights are defined in `governance.md`.

Rules:
- **One decision = one owner**
- **No silent approvals** where approval is required
- **Escalation is expected**, not a failure
- **Decisions are documented and executed**

Documents may not redefine decision rights.

---

## Change Process

1. All changes are made via pull request
2. Each change must state:
   - What is changing
   - Why it is changing
3. Reviewer requirements follow `governance.md`
4. Approved changes are merged to `main`

Deprecated documents are archived, never deleted.

---

## RFCs (Decision Memory)

RFCs are required for:
- Strategy changes
- Target audience changes
- Product direction changes
- Rule or governance changes

RFCs explain **why** a decision was made.

Current documents describe **what is true now**.

---

## Review Cadence

| Document | Review Cycle |
|--------|--------------|
| Constitution | 12 months |
| Governance | 12 months |
| Strategy | 6 months |
| Rules | 6 months |
| Target Audience | 6 months |
| Roadmap | 3–6 months |

Documents past their review date are considered **untrusted**.

---

## Usage Rule

This repository is mandatory context for:
- Strategic decisions
- Product decisions
- Hiring and org design
- External communication
- Automation and AI systems

If context is missing:
- Escalate
- Decide
- Write it down
- Move on

