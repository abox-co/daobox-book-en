---
id: dd40b8cc-13e1-47a1-b47e-2072c4d38e68
title: Features
created_at: 2026-09-05T07:06:20+08:00
updated_at: 2026-09-16T23:19:33+08:00
---


# Features

{#private}
Below is a block-by-block list of what DaoBox **already ships**. No click-by-click how-tos—scan it, and see what you need. For what the product is solving and how people typically use it, see [[intro]]; for concrete scenarios, see [[user-cases]]; for common questions, see [[faq]].

## 1. Workspace & entry

- Open / create a workspace (a local folder is the library)
- Recent workspaces
- Multiple windows; open a folder in a new window
- Drag-and-drop to open Markdown or a folder
- System “Open with DaoBox” for Markdown (on by default)
- Loose files outside a library and Guest windows (no full workspace required first)
- DaoBox Cloud: device-authorized sign-in; open the cloud home from Settings
- Clone from a cloud Git repo, then open
- Welcome page

## 2. Files & assets

- File tree: new file / folder, rename, delete, refresh, reveal in tree
- Single-click expand / collapse for folders
- Multi-select and batch actions in the file tree
- Deletes go to the system Trash (recoverable)
- Show in system file manager
- Copy absolute / relative path
- Directory listing filters (hide-style rules)

## 3. Open & read

- Markdown: preview only / source only / split view
- Plain text and common config files: text editing (with word wrap)
- Preview for images, PDF, HTML, audio, video
- Fallback preview for other types

## 4. Markdown authoring

- Save / save all; reload
- Pop-up edit layer; block-level editing
- Swap split panes, synced preview scrolling, word wrap
- Multi-cursor and column select; status bar shows selection count and one-click collapse
- Insert formatting: headings, bold / italic / strikethrough, inline code, lists, task lists, quotes, code blocks, tables, horizontal rules, links, internal links
- Completions: wikilink / internal link, extended attributes, snippets
- Follow links (including `#heading` anchors); click in preview to jump to the edit location
- Frontmatter maintained on create and save
- Trailing hard-break spaces shown as faint dots

## 5. Find & navigate

- Command palette: go to file / search commands / search body text (switchable modes)
- Quick Open accepts absolute paths
- Body search can narrow by folder, tags, and more
- Sidebar find & replace (including folder scope and replace all)
- In-file find / replace; find in preview
- Outline
- Backlinks (opening Markdown can go straight to inline edit)
- Markdown file list

## 6. Layout & UI

- Sidebar multi-view switching
- Bottom bar (Output / Problems / Publish)
- Dock split panes and tabs (close others, close to the right, etc.)
- Four-way splits (up / down / left / right); orientation can follow window aspect
- Custom title bar and app menu
- Status bar, notifications, and confirmations
- UI zoom

## 7. Private content & in-library preview

- Private zone markers
- Title-bar toggle: show / hide private zones in the library
- Private content is hidden from readers in site preview and export
- In-library HTML and local asset preview (separate from site preview)

## 8. Document export & single-post sharing

- Export preview to PDF / print preview
- PDF: multi-column (up to 3), landscape, base body font size
- Export to Word (optional save-path picker)
- Publish a single post to youlog.net (optional expiry)

## 9. Publish & site output

- Start / stop site preview (live render pipeline)
- Export a static site
- Bottom-bar Publish: export → static preview of the build → push to a remote publish branch
- Serve Dist output (separate from live preview); status bar shows the URL and can stop it
- Push reuses the workspace Git remote; choose branch / directory; optionally push tags too
- Recent push history; publish logs go to Output
- In-app browser for site pages (address bar, reload, find-in-page)
- Edit `everkm.yaml`, `daobox.json`
- Workspace preview watching, path prefix, publish-related, and other settings
- Different templates map to different site shapes (e.g. Blog, Book); content still comes from the current workspace

## 10. Git versioning

- Sidebar: changes, history, sync
- Init repo, status, commit, diff, discard changes (drag-select and bulk discard in the change list)
- Tags, inspect a commit, conflict-handling entry points
- One-click sync with clearer conflict handling
- Remote auth: system credentials / token / SSH; proxy
- Clone wizard (open a library from the cloud)
- Soft-deleted cloud repository names can be reused

## 11. Diagnostics & disk sync

- Problems (list, locate, expand / collapse)
- Output panel
- In-edit diagnostics (e.g. internal-link related)
- Invalid frontmatter is reported as a problem without stopping the whole batch
- External changes: reload / compare / ignore
- Save conflict handling
- Coordination when a file is deleted on disk (recreate or close)
- Unsaved changes prompt on quit
- Open log directory; diagnostic toggles for troubleshooting

## 12. Settings & preferences

- Language (中文 / English)
- Default editor layout (preview / source / split)
- View shortcuts, record remaps, restore defaults
- Global: Git SSH keys, proxy, etc.
- Workspace: preview, private-zone related, Git remote & auth, site & publish related

## 13. Other

- About
- Auto-update (in-app release notes when checking for updates)
- Theme and related site asset capabilities
- Aligned with the CLI publish engine (desktop preview / export match its semantics)
