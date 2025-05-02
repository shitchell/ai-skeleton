# cycle_end_of_feature.md

## 🧹 Post-Feature Cycle
When a feature has been completed (meaning: all scoped work is complete and tests pass), follow this process to close the loop.

---

### ✅ 1. Confirm Completion
- All tests pass?
- All scoped work complete?
- All logs updated?

---

### 🧽 2. Prune & Consolidate
- Review `development_log.md` and prune any redundant or resolved items
- Mark stale sections in other docs with `<!-- prune-needed -->`
- Condense notes into updated docs (e.g. update `implementation_plan.md` or `component_architecture.md`)

---

### 🧠 3. Capture Learnings
- Add any non-obvious lessons to `lessons_learned.md`
- Note any relevant design patterns, edge cases, or surprises
- Log any newly discovered or resolved fracture points

---

### 💡 4. Reflection
- What worked surprisingly well?
- What could be smoother?
- What blind spots did we encounter?
- Were there any misalignments between values and decisions?
- If there were issues, how could they have been avoided given our limited knowledge at the beginning?

Record this reflection in `reflections.md`.

---

### 🧱 5. Update Long-Term Docs (if needed)
- If project direction changed, update `project_specs.md`
- If architecture shifted, update diagrams or `design_decisions.md`
- If constraints or values evolved, update them explicitly

---

### 📈 6. Plan Next Steps
- Define the next high-level objective or set of components
- Create a new entry at the top of `development_log.md`

---

### 🔄 Navigation
- If more work remains, return to [cycle_development_process.md](./cycle_development_process.md)
- If the project is complete, continue to [cycle_end_of_project.md](./cycle_end_of_project.md)
