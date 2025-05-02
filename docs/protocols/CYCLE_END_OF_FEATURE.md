# CYCLE_END_OF_FEATURE.md

## 🧹 Post-Feature Cycle
When a feature has been completed (meaning: all scoped work is complete and tests pass), follow this process to close the loop.

---

### ✅ 1. Confirm Completion
- All tests pass?
- All scoped work complete?
- All logs updated?
- Verify implementation is fully reflected in [MAP.md](../project/blueprint/MAP.md)

---

### 🧽 2. Prune & Consolidate
- Review [DEVELOPMENT_LOG.md](../project/workspace/DEVELOPMENT_LOG.md) and prune any redundant or resolved items
- Review [SCRATCH.md](../project/workspace/SCRATCH.md) and determine which items:
  - Need immediate resolution before transitioning
  - Can be incorporated into existing documentation
  - Should remain in [SCRATCH.md](../project/workspace/SCRATCH.md) for future consideration
  - Require creating new documentation patterns
- Mark stale sections in other docs with `<!-- prune-needed -->`
- Condense notes into updated docs (e.g. update [IMPLEMENTATION_PLAN.md](../project/workspace/IMPLEMENTATION_PLAN.md) or [COMPONENT_ARCHITECTURE.md](../project/blueprint/COMPONENT_ARCHITECTURE.md))

---

### 🧠 3. Capture Learnings
- Add any non-obvious lessons to [LESSONS_LEARNED.md](../project/workspace/LESSONS_LEARNED.md)
- Note any relevant design patterns, edge cases, or surprises
- Log any newly discovered or resolved fracture points in [FLEX_POINTS.md](../project/blueprint/FLEX_POINTS.md)

---

### 💡 4. Reflection
- What worked surprisingly well?
- What could be smoother?
- What blind spots did we encounter?
- Were there any misalignments between values and decisions?
- If there were issues, how could they have been avoided given our limited knowledge at the beginning?

Record this reflection in [REFLECTIONS.md](../project/workspace/REFLECTIONS.md).

---

### 🧱 5. Update Long-Term Docs (if needed)
- If project direction changed, update [PROJECT_SPECS.md](../project/identity/PROJECT_SPECS.md)
- If architecture shifted, update diagrams or [DESIGN_DECISIONS.md](../project/identity/DESIGN_DECISIONS.md)
- If constraints or values evolved, update them explicitly
- Update [MAP.md](../project/blueprint/MAP.md) to reflect any changes to the project structure

---

### 🔄 5b. System Coherence Check
- Run [COHERENCE_CHECK.md](./COHERENCE_CHECK.md) to validate end-to-end coherence
- Verify that all implemented features can be traced to project goals in [MAP.md](../project/blueprint/MAP.md)
- If this feature introduced new process patterns or documentation structures, run [SYSTEM_AUDIT.md](./SYSTEM_AUDIT.md)
- Resolve any detected gaps before proceeding

---

### 📈 6. Plan Next Steps
- Define the next high-level objective or set of components
- Create a new entry at the top of [DEVELOPMENT_LOG.md](../project/workspace/DEVELOPMENT_LOG.md)
- Update [MAP.md](../project/blueprint/MAP.md) with the planned next steps to maintain forward coherence

---

### 🔄 Navigation
- If more work remains, return to [CYCLE_DEVELOPMENT_PROCESS.md](./CYCLE_DEVELOPMENT_PROCESS.md)
- If the project is complete, continue to [CYCLE_END_OF_PROJECT.md](./CYCLE_END_OF_PROJECT.md)