# 📚 Project Documentation Overview

This directory houses all documentation related to project structure, planning, decision-making, and AI/human workflows.

Documentation is split into three main categories:

---

<!-- Add a section for our development protocols here -->
## 🏗️ `protocols/`
Rarely changing documents that define the **protocols** and **guidelines** for development — how we solve plan and solve problems.
- [CYCLE_DEVELOPMENT_PROCESS.md](./protocols/CYCLE_DEVELOPMENT_PROCESS.md) — Daily development loop used throughout active work.
- [CYCLE_END_OF_FEATURE.md](./protocols/CYCLE_END_OF_FEATURE.md) — Checklist for pruning and reflection at the end of a feature.
- [CYCLE_END_OF_PROJECT.md](./protocols/CYCLE_END_OF_PROJECT.md) — Wrap-up flow and final project consolidation.
- [DOCS_MAINTENANCE.md](./protocols/DOCS_MAINTENANCE.md) — Rules for pruning, archiving, and doc clarity.
- [SETUP_PLANNING.md](./protocols/SETUP_PLANNING.md) — Initial setup and planning for a new project.
- [SYSTEM_AUDIT.md](./protocols/SYSTEM_AUDIT.md) — Validates the integrity of the overall documentation system.

<!-- Add a section for organization standards here -->
## 📜 `standards/`
Documentation that defines the **standards** and **conventions** for the project.
- [AI_GUIDANCE.md](./standards/AI_GUIDANCE.md) — Guidelines for AI when deciding on next steps.
- [ARCHITECTURE_PATTERNS.md](./standards/ARCHITECTURE_PATTERNS.md) — Common patterns and practices for architecture.
- [HUMAN_AI_COLLABORATION.md](./standards/HUMAN_AI_COLLABORATION.md) — Guidelines for effective human-AI collaboration.

<!-- Add a section for the project identity and values here -->

## 🧭 `project/identity/`
Slow-changing docs that define the **identity**, **values**, and **process** of the project.

- [PROJECT_SPECS.md](./project/identity/PROJECT_SPECS.md) — Goals, values, philosophy, constraints, and fracture points.
- [DESIGN_DECISIONS.md](./project/identity/DESIGN_DECISIONS.md) — Key architectural decisions and their rationale.

<!-- Add a section for the overarching project blueprint here -->

## 🗺️ `project/blueprint/`
High-level documents that outline the **overarching project blueprint**.

- [PROJECT_BLUEPRINT.md](./project/blueprint/PROJECT_BLUEPRINT.md) — High-level overview of the project, its components, and their interactions.
- [ARCHITECTURE.md](./project/blueprint/ARCHITECTURE.md) — Detailed architecture of the project, including diagrams and explanations.
- [ARCHITECTURE_DECISIONS.md](./project/blueprint/ARCHITECTURE_DECISIONS.md) — Key architectural decisions and their rationale.
- [COMPONENT_ARCHITECTURE.md](./project/blueprint/COMPONENT_ARCHITECTURE.md) — In-progress structural blueprints and dependencies.
- [MAP.md](./project/blueprint/MAP.md) — Traceable system map linking goals to components.
- [FLEX_POINTS.md](./project/blueprint/FLEX_POINTS.md) — Areas of intentional flexibility in the architecture.

---

## 🔄 `project/workspace/`
Frequently updated documents that capture **ongoing development**.

- [DEVELOPMENT_LOG.md](./project/workspace/DEVELOPMENT_LOG.md) — Session-by-session dev entries, decisions, and context.
- [LESSONS_LEARNED.md](./project/workspace/LESSONS_LEARNED.md) — Collected mistakes and insights from the journey.
- [IMPLEMENTATION_PLAN.md](./project/workspace/IMPLEMENTATION_PLAN.md) — Outline of upcoming or WIP features and priorities.
- [SCRATCH.md](./project/workspace/SCRATCH.md) — Notes and ideas that are not yet formalized.
- [README.md](./project/workspace/README.md) — Onboarding info for contributors or fresh context for the AI.

---

## 📦 `archived/`
Finalized, deprecated, or historical artifacts.

- [example_diagram.puml](./archived/example_diagram.puml) — PlantUML sample diagram.
- [placeholder.txt](./archived/placeholder.txt) — Reminder to archive rather than delete when pruning.
- [ARCHIVAL_LOG.md](./archived/ARCHIVAL_LOG.md) — Record of archived documents and their reasons for archiving.

---

## 🚦 Suggested Entry Points

| Situation                        | Start With                            |
|----------------------------------|----------------------------------------|
| You're planning your next task   | [CYCLE_DEVELOPMENT_PROCESS.md](./protocols/CYCLE_DEVELOPMENT_PROCESS.md) |
| You just finished a feature      | [CYCLE_END_OF_FEATURE.md](./protocols/CYCLE_END_OF_FEATURE.md) |
| You're wrapping the whole project| [CYCLE_END_OF_PROJECT.md](./protocols/CYCLE_END_OF_PROJECT.md) |
| You're new to the project        | [PROJECT_SPECS.md](./project/identity/PROJECT_SPECS.md) → [README.md](./README.md) |
| Something feels wrong/confusing  | [DOCS_MAINTENANCE.md](./protocols/DOCS_MAINTENANCE.md) or [LESSONS_LEARNED.md](./project/workspace/LESSONS_LEARNED.md) |
| Need to validate documentation   | [VALIDATION.md](./VALIDATION.md) and [SYSTEM_AUDIT.md](./protocols/SYSTEM_AUDIT.md) |

---

🧠 **Reminder**: This system is designed to be AI-friendly, minimizing context loss while retaining high signal-to-noise clarity across all project stages. Don't hesitate to emit `<!-- prune-needed -->` in any doc that needs cleanup.


---

## 🧠 Design Protocols
- [COHERENCE_CHECK.md](./protocols/COHERENCE_CHECK.md): Ensures all project work aligns with defined goals and architecture.
- [MAP.md](./project/blueprint/MAP.md): Traceable system map linking goals to components.
- [SYSTEM_AUDIT.md](./protocols/SYSTEM_AUDIT.md): Validates the integrity of the overall documentation system.
- [VALIDATION.md](./VALIDATION.md): Tools and guidelines for linting, link checking, and doc formatting.