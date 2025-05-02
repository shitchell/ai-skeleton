# AI_CODING_GUIDANCE.md

## 📘 Purpose
This document helps align AI development with human expectations, by outlining:
- Preferred paradigms for different problem types
- File structures that aid LLM reasoning
- Definitions of key terms (like declarative, composable, etc.)
- When and how to blend different coding styles

---

## 🧠 Definitions (for humans AND AI)

### 🟩 Declarative
> Code that describes *what* you want, not *how* to do it.

**Example:**
```js
const filtered = users.filter(u => u.isActive);
```
vs
```js
let filtered = [];
for (let i = 0; i < users.length; i++) {
  if (users[i].isActive) filtered.push(users[i]);
}
```
**Why it helps AI:** Shorter, more expressive, easier to refactor or re-target.

---

### 🟩 Composable
> Code where small parts can be combined in flexible ways.

**Example (functional composition):**
```js
const cleanInput = compose(trim, normalize, lowercase);
```
**Why it helps AI:** Encourages reuse, modular reasoning, and fewer side effects.

---

### 🟩 Semantically Shallow
> Code that doesn't require deep state tracking or mental gymnastics to understand.

**Shallow example:**
```js
const result = addTax(price);
```
**Deep example:**
```js
class CartItem extends Purchasable implements Serializable {
  constructor(config) {
    super();
    this.discountRate = config.discountRate || getDefaultRate();
  }
}
```
**Why it helps AI:** Fewer nested dependencies = easier code synthesis and debugging.

---

## 🧩 Problem Types → Paradigm Choices

| Problem Type                   | Paradigm                   | Notes                                  |
|-------------------------------|-----------------------------|----------------------------------------|
| Data transformation           | Functional                  | Prefer pure functions, no mutation     |
| UI + event handling           | Event-driven / Reactive     | Signals, observer, or state stores     |
| Rule-based validation         | Declarative + Functional    | Rules as data + validators as funcs    |
| Plugin systems                | OOP + Registry              | Interface-based loading                |
| CLI or procedural pipelines   | Imperative or Factory       | One-shot flow, explicit step order     |
| Simulation, FSM               | ECS / Actor Model / StateFn | State machines preferred               |

---

## 🧱 File Structure Guidance

| Layer / Role      | Folder Suggestion        | Example Paradigm      |
|------------------|--------------------------|------------------------|
| Core utils       | `src/lib/`               | Functional             |
| State            | `src/state/`             | Signals, Redux, FSM    |
| Components       | `src/components/`        | Declarative + Events   |
| Plugins          | `src/plugins/`           | Factory + OOP          |
| CLI              | `src/cli/`               | Procedural / Factory   |
| Validators       | `src/validators/`        | Declarative + Func     |

---

## 🔀 When to Blend Paradigms
It’s okay to blend as long as:
- You keep **one dominant paradigm per file or module**
- You document the style boundaries (e.g. "plugin system uses factory")
- You don’t cross-contaminate (e.g. don't mix event emitters and factories inside one class)

---

## 🔄 Navigation
- Back to process loop → [CYCLE_DEVELOPMENT_PROCESS.md](../persistent/CYCLE_DEVELOPMENT_PROCESS.md)
- Org-level design reference → `ARCHITECTURE_PATTERNS.md`, `PROJECT_SPECS.md`, etc.
