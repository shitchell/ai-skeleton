# VALIDATION.md

## 🧪 Purpose

This document describes how to run static checks against your documentation system for structure, correctness, and clarity.

---

## ✅ Tools and What They Check

### 1. [`lychee`](https://github.com/lycheeverse/lychee)
- Checks: broken links (internal and external)
- Run: `lychee docs/**/*.md`

### 2. [`markdownlint`](https://github.com/DavidAnson/markdownlint)
- Checks: markdown formatting, consistency, structure
- Run: `markdownlint docs/`

### 3. [`markdown-link-check`](https://github.com/tcort/markdown-link-check)
- Alternative to lychee if you want a simpler link checker
- Run: `markdown-link-check -c config.json docs/**/*.md`

### 4. [`vale`](https://vale.sh/)
- Checks: grammar, style, and tone for English prose
- Configurable for voice, clarity, etc.
- Run: `vale docs/`

---

## 💡 Best Practices for Valid Markdown

- Always link other files like `[PROJECT_SPECS.md](../identity/PROJECT_SPECS.md)` — not just `PROJECT_SPECS.md`
- Avoid dangling references or "See TODO.md" without a real file
- Use fenced code blocks (```) with a language identifier
- Prefer bullets over inconsistent indentation

---

## 🧠 Optional Integration

You can run these checks automatically in CI or pre-commit with a tool like [`pre-commit`](https://pre-commit.com/) or GitHub Actions.

---

## 📁 Related Files

- [COHERENCE_CHECK.md](./protocols/COHERENCE_CHECK.md)
- [SYSTEM_AUDIT.md](./protocols/SYSTEM_AUDIT.md)
- [FLEX_POINTS.md](./project/blueprint/FLEX_POINTS.md)
- [MAP.md](./project/blueprint/MAP.md)