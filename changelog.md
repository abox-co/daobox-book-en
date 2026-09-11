---
id: 92fd8293-0ccb-4e9f-b3d3-8d7d85573c8e
created_at: 2026-09-11T11:57:10+08:00
updated_at: 2026-09-11T11:57:10+08:00
title: Changelog
slug: changelog
---

{#private}
Spec reference: /Users/dayu/Coder/everkm/everkm2/global_km/changlog-spec.md

## v0.4.0 (2026-09-11)

- **Editing & multi-select**
  - Multi-cursor and column select: Alt-click to add a cursor, Alt-drag for a rectangle; Cmd/Ctrl+D to select the next match.
  - Status bar shows selection count; click to collapse back to a single cursor.

- **Split layout**
  - Tabs and the more menu can split in all four directions.
  - Split orientation can follow the window aspect; the divider is easier to drag.

- **Files & changes**
  - Deletes go to the system Trash, so accidental removals can be restored.
  - File tree supports multi-select batch actions; the changes list supports drag-select and bulk discard.

- **Sync & remote edits**
  - One-click sync handles conflicts more completely; local unpushed state stays fresher.
  - Remote edits merge line-by-line and try to keep your scroll position.

- **Writing polish**
  - Frontmatter is maintained automatically on create and save.
  - Trailing hard-break spaces show as faint dots, so they’re harder to leave or delete by mistake.

- **Open & preview**
  - Missing files get a clear empty state with a retry path.
  - Preview theme switching and export output are cleaner.

## v0.3.0 (2026-09-08)

- **DaoBox Cloud**
  - Device-authorized sign-in and cloud connection; open the cloud home from Settings.
  - Pick a cloud repo, clone it, and open it as a workspace.

- **Site publishing**
  - Push a static site; the console shows deployments and repos.
  - Status-bar publish and push flows are clearer.

- **Welcome page**
  - Shows a remote summary and links to the cloud home.
  - Reveal the workspace folder in the system file manager.

- **Large files**
  - Cloud sync supports large-file transfer.

## v0.2.2 (2026-09-06)

- **Preview layout**
  - One-click switch among preview / source / split, while trying to keep your place on screen.
  - Editor cursor maps to a left edge on the matching preview block; internal-link follow and footnote jumps are more reliable.

- **In-app browser**
  - Open site pages in-app, with address bar, refresh, and find-in-page.

- **Publish**
  - New publish panel for static preview push; publish history is easier to scan.

- **Help & docs**
  - Welcome page and Help menu open the user docs; About has fuller contact info.

- **Open & windows**
  - Paths queued at cold start are no longer lost; opening another library defaults to a new window.
  - Closing the last window quits the app.

## v0.2.1 (2026-09-02)

- **Windows**
  - “Show in Explorer” works; path display is cleaner.
  - Illegal filename characters are blocked on create or rename.
  - Exports that include math no longer fail.

- **Updates & creating files**
  - The About dialog no longer blocks “Check for Updates.”
  - When creating across sidebars, the name field focuses reliably.

## v0.2.0 (2026-09-01)

- **Version control**
  - Clone, commit, sync, history, and tags.
  - Import SSH keys, discard changes, and preview diffs.

- **Writing workspace**
  - Three-pane shell with a custom title bar.
  - Markdown split preview, writing toolbar, and internal-link navigation.

- **Find & navigate**
  - Quick Open, global find & replace, outline, backlinks, and note list.

- **Completions**
  - Smart completions for internal links, image links, and extended attributes.

- **Multi-window & external changes**
  - Multiple windows, each with its own workspace.
  - Conflict prompts and merge when files change outside the app.

- **Notifications & diagnostics**
  - Layered status-bar feedback; Problems diagnostics with auto-fix.

- **Themes**
  - Theme folders can live in the library and be tracked with Git.

## v0.1.2 (2026-08-25)

- **Install & updates**
  - Smaller installers—faster to download and install.
  - Check for Updates surfaces this release’s highlights.
  - Assorted auto-update and install fixes.

## v0.1.1 (2026-08-25)

- **Auto-update**
  - First auto-update and packaged release pipeline.

## v0.1.0 (2026-08-25)

- **Initial release**
  - First DaoBox desktop build.
