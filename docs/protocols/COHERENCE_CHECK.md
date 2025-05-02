
# COHERENCE_CHECK.md

## 🧭 Purpose
This protocol defines how to ensure every change, plan, or implementation is logically and structurally aligned with the rest of the project.

> The goal is to preserve coherence across all design layers — from high-level goals to individual components.

This check should be run:
- At the start of the project (as part of setup)
- Before writing any new code
- After learning something new, identifying a risk, or proposing a major change
- Before finalizing a feature or milestone

---

## 🔄 The Coherence Check Loop

### Step 1: Declare Intent
> What are you trying to do?
- New feature?
- Refactor?
- Update a test?
- Revise a requirement?

Write this clearly in `DEVELOPMENT_LOG.md` or explain to the AI agent.

---

### Step 2: Trace Dependencies (Up the Chain)
Using `MAP.md`, determine what this change depends on:
- Which **goal(s)** does it serve?
- What **use case(s)** or **user story** supports it?
- Which **requirement** does it fulfill?
- What **component(s)** are involved?

If any parent node is **undefined, unclear, or contradictory**, go to Step 4.

---

### Step 3: Check for Fractures
Look for:
- Misalignments between architecture and goals
- Missing links in the `MAP.md`
- Incomplete use cases or undefined flex points
- Ambiguities in `PROJECT_SPECS.md`, `USER_REQUIREMENTS.md`, or `COMPONENT_ARCHITECTURE.md`

If the structure supports your intent: ✅ Proceed to implementation.

If not: 🔍 Continue.

---

### Step 4: Resolve or Define Flex Point
If something is missing, do one of the following:
- **Resolve** it: define the missing requirement, story, or component
- **Flex it**: add it to `FLEX_POINTS.md` with the following:
  1. Why we chose to leave it undefined
  2. Possible coherent branches
  3. Possible incoherent outcomes
  4. Risk level
  5. When it must be resolved

Then return to Step 3.

---

### Step 5: Confirm Downward Impact
Ensure any change you make:
- Is reflected in `MAP.md`
- Doesn’t break coherence with any child nodes
- Is reflected in the affected component, test, or logic

Update diagrams or `DESIGN_DECISIONS.md` if this change alters existing patterns.

---

## 🧠 What Is a Gap?
A **gap** is:
- A node in the project map with no definition or known contradictions
- A missing user behavior, requirement, or tech decision
- A feature or path whose purpose can’t be traced up to a goal

Gaps **must** be resolved or documented before implementation.

---

## 🔁 Flowchart

```plantuml
@startuml
!include COHERENCE_CHECK_FLOWCHART.puml
@enduml
```

---

## 📄 References
- `project/blueprint/MAP.md`
- `project/blueprint/FLEX_POINTS.md`
- `project/identity/PROJECT_SPECS.md`
- `project/identity/DESIGN_DECISIONS.md`
- `project/blueprint/COMPONENT_ARCHITECTURE.md`
- `project/workspace/DEVELOPMENT_LOG.md`

---

## 🔄 Navigation
- Begin planning: [SETUP_PLANNING.md](./SETUP_PLANNING.md)
- Proceed to daily dev loop: [CYCLE_DEVELOPMENT_PROCESS.md](./CYCLE_DEVELOPMENT_PROCESS.md)
