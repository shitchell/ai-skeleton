# PROJECT_SPECS.md

## 🧭 Project Overview
- **Project Name**: [Your Project Name Here]
- **Short Summary**: [What does this project do? One-liner.]
- **Environment**: [Web, CLI, API, etc.]
- **Key Users**: [Who is this for?]

---

## 🎯 Overarching Goals
- [List high-level outcomes the project aims to achieve]
- [These should change rarely — only when vision or purpose changes]

---

## 💡 Core Values
- [Principles that should guide every decision — e.g., "simplicity over extensibility"]
- [Could include dev philosophy, UX priorities, transparency, etc.]

---

## 🧘 Spirit / Philosophy
- [Freeform descriptions of "how" this project should feel — e.g., hacker ethos, educational tool, welcoming design, etc.]

---

## 🚫 Project Constraints
- [ ] Must run offline
- [ ] Must support plugins
- [ ] Must use no external dependencies
- [ ] Must be testable with Playwright / Vitest
- [ ] Must support async operations
- [ ] Minimum Node.js version: 16
- [ ] Low memory available
- [ ] ...

(Only include constraints that are fundamental to the project's identity.)

---

## 🔀 Flex Points
These are areas we intentionally design for future change:
- [e.g., Plugin system should allow new validator types]
- [e.g., UI theme engine should support overrides but default to system style]

---

## ⚠️ Known Fracture Points
Design limitations we **know** exist but are accepting for now:
- [e.g., CLI argument parser is not reusable outside main module]
- [e.g., Validation engine assumes file-based input only]

Include rationale for why these are tolerated.

---

## ❓ Undefined Fracture Points
Ambiguities or potential architectural landmines that we haven’t solved yet:
- [e.g., What happens if multiple plugins validate the same file in conflicting ways?]
- [e.g., Are async validators allowed to mutate shared state?]

These should **ideally be reviewed regularly** and may be migrated to another document (like `LESSONS_LEARNED.md`) as they're resolved.

---

## 🔗 References
- Architecture diagrams
- Prototypes / Figma
- Similar open-source projects

---

**NOTE**: This file should be updated only when the project's **core identity** changes — goals, values, foundational assumptions, or known architectural commitments.

---

### 🔄 Workflow Navigation
- Proceed to [CYCLE_DEVELOPMENT_PROCESS.md](./CYCLE_DEVELOPMENT_PROCESS.md) to begin iteration cycles.
- See [CYCLE_END_OF_FEATURE.md](./CYCLE_END_OF_FEATURE.md) and [CYCLE_END_OF_PROJECT.md](./CYCLE_END_OF_PROJECT.md) for end-cycle rituals.
