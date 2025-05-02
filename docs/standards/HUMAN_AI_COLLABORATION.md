# HUMAN_AI_COLLABORATION.md

## 🤝 Purpose
This document outlines how human and AI agents can work together to maximize clarity, momentum, and alignment toward the goals defined in [PROJECT_SPECS.md](../project/identity/PROJECT_SPECS.md).

---

## 🧠 Core Assumption
Humans and AIs are not interchangeable. Each has strengths and weaknesses. The goal is not to divide labor equally, but to **allocate responsibility where it's best served**.

---

## 🧍 Human Strengths
- **Big-picture judgment**: Values, tradeoffs, intention, and emotional resonance
- **Design intuition**: Recognizing when patterns "feel wrong" or are misaligned
- **Edge-case awareness**: Knowing historical failures, nuance, and real-world complexity
- **Ethical responsibility**: Understanding harm, fairness, and unintended consequences
- **Creative synthesis**: Blending ideas from disparate contexts into novel solutions

---

## 🤖 AI Strengths
- **High-speed iteration**: Generating structured code and boilerplate rapidly
- **Pattern recognition**: Identifying and following repeatable design motifs
- **Context-sensitive response**: Adapting to project values and goals when scoped well
- **Detail-oriented memory** (within limits): Recalling and repeating instructions precisely
- **Task decomposition**: Breaking down goals into smaller, actionable subtasks

---

## 🔁 Alignment Principles

### ✅ Shared Responsibility
| Task Type                         | Primary Agent  | Notes |
|----------------------------------|----------------|-------|
| Architecture + Design Intent     | Human          | Claude may assist with diagrams or rationalization |
| Code Generation                  | AI             | Prefer declarative + composable patterns |
| Refactoring + Simplification     | AI (with review) | Use [LESSONS_LEARNED.md](../project/workspace/LESSONS_LEARNED.md) to capture rationale |
| Test Writing                     | AI             | Include edge cases and manual test descriptions |
| Error Diagnosis                  | Both           | AI can trace logic; humans validate assumptions |
| Documentation                    | AI drafts / Human prunes | Claude generates; humans condense or correct |
| Decision Review + Philosophy     | Human          | Ensure continued alignment with [PROJECT_SPECS.md](../project/identity/PROJECT_SPECS.md) |

---

### 🔁 Iteration Loop
1. Human initiates a plan (via [DEVELOPMENT_LOG.md](../project/workspace/DEVELOPMENT_LOG.md) or issue)
2. AI proposes implementation
3. Human reviews direction and constraints
4. AI develops code + docs + tests
5. Human/AI review outcome; prune docs if needed
6. Loop or shift to feature/project closure

---

## 🧠 Human-AI Interface Norms
- Use `<!-- clarify -->` or `<!-- prune-needed -->` comments to indicate questions or cleanup points
- AI should emit **navigation notes** at the end of every output (e.g. "continue in [CYCLE_DEVELOPMENT_PROCESS.md](../protocols/CYCLE_DEVELOPMENT_PROCESS.md)")
- Human should check [PROJECT_SPECS.md](../project/identity/PROJECT_SPECS.md) if vision, values, or constraints are in question
- AI should reference [LESSONS_LEARNED.md](../project/workspace/LESSONS_LEARNED.md) and [DESIGN_DECISIONS.md](../project/identity/DESIGN_DECISIONS.md) when similar patterns reappear

---

## 🪵 Misalignment Signals
| Symptom                            | Possible Source                |
|-----------------------------------|-------------------------------|
| Code is technically valid but feels off | AI over-prioritized pattern, not philosophy |
| Docs balloon without direction     | AI iterated without context or review |
| Features drift from project values | Human failed to ground AI in specs |
| Errors persist across iterations   | Misunderstood feedback loop or testing layer |

---

## 🧭 When in Doubt
- Check [PROJECT_SPECS.md](../project/identity/PROJECT_SPECS.md) — are we still aligned?
- Check [CYCLE_DEVELOPMENT_PROCESS.md](../protocols/CYCLE_DEVELOPMENT_PROCESS.md) — did we skip a step?
- Log confusion in [DEVELOPMENT_LOG.md](../project/workspace/DEVELOPMENT_LOG.md) — future clarity begins with traceability

---

**The best collaboration isn't faster — it's clearer.**
We build better together by playing to our strengths.

---

## 📄 References
- [HUMAN_AI_COLLABORATION.md](../standards/HUMAN_AI_COLLABORATION.md)