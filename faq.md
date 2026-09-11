---
id: 26bf7641-b835-4d9f-98c0-95924a88732f
title: FAQ
created_at: 2026-09-05T07:06:20+08:00
updated_at: 2026-09-11T11:57:10+08:00
---



# FAQ

## 1. Is DaoBox a note app or a site generator?


Neither, exclusively. It’s a **local Markdown file knowledge base**: the home base is writing and accumulation; when you need to, you preview or export the same library as a site. It’s fine if you only take notes. If you only want a pure SSG and don’t care about day-to-day writing, it’s usually not the best fit.

## 2. How does it compare to tools like Obsidian?


There’s overlap in local Markdown, linking, and search. DaoBox puts more weight on **taking the same file tree through to site preview / export**, and on private content that stays hidden when you publish—not on being a plugin-powered “do everything” note workstation. If you rarely need a site and you’re mostly comparing editing feel, try it yourself and decide.

## 3. What about Hugo / Jekyll and similar tools?


Those shine at site engineering; day-to-day writing often happens in a separate editor. DaoBox keeps everyday reading/writing and preview/export in one workspace, so you don’t pay the “write in one place, publish from another” tax. Deep theme and template customization may still mean touching config and the theme system—the app covers common settings, but it won’t pretend you never need to understand sites at all.

## 4. Where is my content stored? Will it be locked into a proprietary format?


In the local folder you choose—ordinary files. Notes aren’t sealed into an app-only library. You can switch editors, use Git, or copy the whole folder.

## 5. Do I have to use Git?


No. You can open a library, write, preview, and export without Git. Git is optional for versioning and remote sync; use it from the sidebar when you need it.

## 6. Is there cloud sync or account login?


There’s no “sign in → cloud note library” product. Remote backup and multi-machine collaboration go through *your* Git remotes (and credential settings)—not a content cloud hosted by DaoBox.

## 7. Can multiple people edit the same document in real time?


No. It’s built for individuals (or small teams collaborating via Git) working on local files—not a collaborative doc with multiplayer cursors.

## 8. How do private content and publishing relate?


Private markers stay in the source. In the library you can show or hide them. In site preview and export, those parts never reach readers. So one draft can hold both “for me” and “for readers.”

## 9. Do I need to know how to build sites or edit templates?


Not for day-to-day accumulation. Open a folder and write. Site-related steps (preview, export, picking a template, editing `everkm.yaml` / `daobox.json`) are the path you take when you’re ready to output; go deeper into themes only when you want a custom look.

## 10. There’s a lot here—where should I start?


See whether [[intro]] matches your problems; skim [[features]] and check what you need; compare situations in [[user-cases]]. You don’t have to learn the feature list item by item.
