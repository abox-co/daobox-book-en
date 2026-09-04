---
id: 7ac1cdae-61ff-40ff-a16a-e196c9d1bf7e
created_at: 2026-09-05T07:06:20+08:00
updated_at: 2026-09-05T07:06:20+08:00
---


# Tips


{id=ai-constraints #private}
## AI constraints

- When adding or rewriting this page, **every level-2 heading (`##`) must include an explicit `{id=…}`** (English kebab-case) so internal links / anchors stay stable; don’t rely on auto-generated title slugs.
- When editing, only update `updated_at` in the frontmatter—don’t change `created_at`.


{id=conventions}
## 0. Conventions

- Unless noted otherwise, `MD` means a Markdown file.
- The shortcut key `Mod` means `Command` on macOS and `Ctrl` on other platforms.

{id=md-quick-edit}
## 1. Quick MD editing

DaoBox is preview-first by design, so Markdown opens as the rendered result. While browsing, if you need a quick change, double-click where you want to edit—a pop-up editor opens and jumps to that spot.
When you’re done, press `Mod+Enter` to save and close,
or `Mod+S` to save only.
Press `Esc` twice to leave the pop-up editor.


{id=private-zone}
## 2. Private zones

Tag blocks with `#tag` in extended attributes. **`#private` is the system default private zone**: it’s stripped during site preview / export, so readers never see it.

```markdown
{#private}
This stays in the source file and is invisible in public rendering.

{#private}
## An entire private section

When placed on a heading, it covers content until the next heading of the same or higher level.
```

Other tags (such as `{#draft}`) can be added as needed; themes / templates control show/hide via an exclude list (`exclude_tags`) without editing the body. In-library writing preview has a separate title-bar toggle for whether excluded zones are shown—independent of public rendering.


{id=md-extensions}
## 3. What we add on top of common MD

Beyond standard Markdown / GitHub Flavored Markdown, DaoBox mainly adds:

### Extended attributes `{…}`

Use curly braces to attach attributes to headings, paragraphs, links, images, and more; separate multiple items with spaces or commas:

| Syntax | Meaning | Example |
|------|------|----|
| `#name` | **Tag** (not an HTML id) | `{#private}` `{#draft}` |
| `.name` | CSS class | `{.notice}` |
| `key` | Flag with no value | `{tc underline}` |
| `key=value` | Key-value; quote values that contain spaces or commas | `{color=red wh=1.5em}` |

Common attachment points:

```markdown
{color=red tc}
# Red, centered heading

A styled [link](https://everkm.cn){color=orangered new-tab}

![Image](./a.png){corner=1em}

I am {color=red}#this# text.
```

Handy shortcut names: `tl` / `tc` / `tr` (alignment), `ul` / `underline`, `color` / `bgcolor`, `pa` / `px` / `py`, `corner`, `wh` / `w` / `h`, `new-tab` (open links in a new tab). For stable in-page anchors, write `{id=section-name}`.

While editing inside `{`, you can complete by prefix: `#` → tags in the library, `.` → classes, bare words → attribute names, `key=` → values already used for that key.

For private zones and tag exclusion, see [[tips#private-zone]].


{#private memo=todo}
### Other common syntax

- Highlight: `==important==`
- Superscript / subscript: `E=MC^2^`, `H~2~O`
- TOC macro: a line by itself `[TOC]`, or a code block with language `macro/toc`
- Embed files: a code block with language `macro/include` (can pull in md / tables / code, etc.)

Prefer internal links `[[…]]` for in-site navigation; see [[tips#inner-link]].


{id=inner-link}
## 4. Internal link forms

Prefer `[[target]]` so the system resolves the final URL—hand-written relative paths can break on export.

```markdown
[[quick-start]]                 # slug or title (case-insensitive)
[[./faq/]]                      # relative to the current file’s directory
[[/docs/guide/quick-start.md]]  # logical path from the library root
[[./page#section-id]]           # with anchor (use a stable {id=...} on the target)
[[./faq/|FAQ]]                  # text after | is the display label
```

Rough match order: slug → title → path. With no prefix, the whole library is searched by path suffix; if multiple hits collide, use `[[./…]]` or `[[/…]]`. A trailing `/` resolves to the directory’s default page. You can also link to non-MD assets such as PDFs and images.

Division of labor with standard links: use `[text](https://…)` for external URLs; use internal links for in-library references.
