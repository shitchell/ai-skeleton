# CYCLE_END_OF_FEATURE.md

## 🧹 Post-Feature Cycle
When a feature has been completed (meaning: all scoped work is complete and tests pass), follow this process to close the loop.

---

### ✅ 1. Confirm Completion
- All tests pass?
- All scoped work complete?
- All logs updated?

---

### 🧽 2. Prune & Consolidate
- Review `DEVELOPMENT_LOG.md` and prune any redundant or resolved items
- Review `SCRATCH.md` and determine which items:
  - Need immediate resolution before transitioning
  - Can be incorporated into existing documentation
  - Should remain in SCRATCH.md for future consideration
  - Require creating new documentation patterns
- Mark stale sections in other docs with `<!-- prune-needed -->`
- Condense notes into updated docs (e.g. update `IMPLEMENTATION_PLAN.md` or `COMPONENT_ARCHITECTURE.md`)

---

### 🧠 3. Capture Learnings
- Add any non-obvious lessons to `LESSONS_LEARNED.md`
- Note any relevant design patterns, edge cases, or surprises
- Log any newly discovered or resolved fracture points

---

### 💡 4. Reflection
- What worked surprisingly well?
- What could be smoother?
- What blind spots did we encounter?
- Were there any misalignments between values and decisions?
- If there were issues, how could they have been avoided given our limited knowledge at the beginning?

Record this reflection in `REFLECTIONS.md`.

---

### 🧱 5. Update Long-Term Docs (if needed)
- If project direction changed, update `PROJECT_SPECS.md`
- If architecture shifted, update diagrams or `DESIGN_DECISIONS.md`
- If constraints or values evolved, update them explicitly

---

### 📈 6. Plan Next Steps
- Define the next high-level objective or set of components
- Create a new entry at the top of `DEVELOPMENT_LOG.md`

---

### 🔄 Navigation
- If more work remains, return to [CYCLE_DEVELOPMENT_PROCESS.md](./CYCLE_DEVELOPMENT_PROCESS.md)
- If the project is complete, continue to [CYCLE_END_OF_PROJECT.md](./CYCLE_END_OF_PROJECT.md)


> 📌 Update your [MAP.md](../project/blueprint/MAP.md) and confirm system-wide consistency via [COHERENCE_CHECK.md](./COHERENCE_CHECK.md).
