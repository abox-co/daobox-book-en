---
id: 9a19fd53-3f9b-4bbb-96fe-9084883803ad
title: DaoBox Book Writing Rules
created_at: 2026-09-05T07:06:20+08:00
updated_at: 2026-09-05T07:06:20+08:00
type: Rule
relates_to:
  - _nav.md
  - intro.md
  - features.md
  - scenarios.md
  - faq.md
---

# DaoBox Book Writing Rules (Rule)

> **Document type**: Rule — writing constraints for the end-user product book under `daobox-book/`; a quick reference for humans and AI collaborating  
> **Scope**: Body pages in this directory and `_nav.md`; does not replace engineering docs under `stuff/km`

---

## 0. Changelog

| Version | Date   | Notes |
|------|--------|------|
| 0.1  | 260902 | First draft: positioning, narrative voice, trade-offs, tone, chapter structure, and acceptance checks |
| 0.2  | 260902 | Structure tightened to four pages: intro / features / use cases / FAQ; multi-chapter narrative split retired |
| 0.3  | 260902 | All body H2 headings use numeric numbering (`## 1. …`) |
| 0.4  | 260905 | English edition translated from the Chinese book |

---

## 1. Document positioning

1.1.1 This book is a user-facing presentation of a product that is **already designed and shipped**—not a brainstorm, not a rewritten research thread, not a dump of a development plan.  
1.1.2 Reader path: **Do the problems and scenarios match → Are the capabilities enough → Do the situations hold together → Are doubts cleared**.  
1.1.3 Not a how-to manual; no step-by-step clicks, full shortcut tables, or settings encyclopedias.  
1.1.4 Engineering design truth lives in `EverkmNote/stuff/km`; this book only covers user-visible capabilities and intent.

---

## 2. Book structure (current)

2.1.1 Navigation source of truth: `_nav.md` (`* [[slug]]`).  
2.1.2 Keep only four pages:

| slug | Title | Role |
|------|------|------|
| `intro` | Introduction | **One page** that clarifies: what problem it solves + who/when typically uses it (brief) |
| `features` | Features | **List everything shipped at a glance**; no how-to |
| `user-cases` | Use Cases | How concrete situations string capabilities together; no step-by-step tutorials |
| `faq` | FAQ | Category comparisons, boundaries, deliberate non-goals, selection doubts |

2.1.3 **Do not** split narrative into chapters like `what-is` / `problems` / `create` / `output` / `not-what` (easy to feel hollow and repetitive). Negative expectations belong in `faq`.  
2.1.4 Scenarios in `intro` are an index only; expand only in `user-cases` so the two pages don’t compete.  
2.1.5 `features` should not spawn sub-nav by default; listing by domain is enough.  
2.1.6 Body frontmatter must include at least `title`, `created_at`, and `updated_at`; when editing, **only update** `updated_at`.

---

## 3. Product narrative

3.1.1 **One-liner**: DaoBox is a local Markdown file knowledge base.  
3.1.2 **Idea** (keep it light): Your knowledge is your files.  
3.1.3 Frame the user relationship as “create and multi-form output”: most days you accumulate; one day you output by angle/form—without a second content library.  
3.1.4 Don’t use external “side A / side B” chapter framing; that language in `km` is engineering coordinates only.  
3.1.5 Don’t write long defenses of “yet another note app” or “pure SSG”; keep comparisons as short FAQ answers.

---

## 4. Content trade-offs

4.1.1 **intro**: Problems + a short scenario list; little feature stacking.  
4.1.2 **features**: Only shipped capabilities; don’t list what’s unfinished.  
4.1.3 **user-cases**: 3–5 concrete situations; name related capabilities briefly.  
4.1.4 **faq**: Questions people actually ask; include “who it’s not for / deliberate non-goals.”  
4.1.5 Capabilities follow the current client—not an outdated plan dressed up as shipping status.

---

## 5. Voice and tone

5.1.1 Everyday language; conversational and natural.  
5.1.2 Avoid: outline-speak, stiff “capability + why” annotation style, R&D jargon (two-sided / coordinate systems), long lectures.  
5.1.3 **H2 headings must be numbered**: `## 1. …`, `## 2. …` (restart at 1 on each page).  
5.1.4 Cross-links use `[[slug]]`.  
5.1.5 Prefer short; if one paragraph works, don’t use three sections.

---

## 6. Relation to implementation / km

6.1.1 Before writing “we have X,” verify the real capability.  
6.1.2 User-visible behavior changes should update the matching page in this book.  
6.1.3 Deliberate non-goals go in `faq` in user language—not engineering ban numbers.

---

## 7. Acceptance checklist

- [ ] Structure is still intro / features / user-cases / faq (four pages)
- [ ] intro doesn’t steal from user-cases; features isn’t a tutorial
- [ ] Reads like a shipped product explanation—not an argument for “whether to build it”
- [ ] Natural tone; no side A/B narrative
- [ ] Unshipped capabilities aren’t written as shipping
- [ ] All H2 headings are numbered
- [ ] `_nav.md` matches body slugs; `updated_at` is current
