---
id: 9ebab549-ae76-4bc2-a96b-18e787209120
title: Use Cases
created_at: 2026-09-05T07:06:20+08:00
updated_at: 2026-09-05T07:06:20+08:00
---


# Use Cases

DaoBox doesn’t prescribe how you should manage knowledge.

Maybe you just want to tame a pile of files. Maybe you’re writing steadily. Or maybe you’ve already built up a lot of content—and one day you suddenly want it to become a website.

Here are some typical ways people use it.

## 01｜I have lots of Markdown files and want to actually use them

You’ve already accumulated Markdown files.

They might be old notes, project docs, reading logs, or content migrated from another tool. They already live in a folder on your computer—they’ve just grown hard to browse and find over time.

You don’t want to import them into a new database just to use them.

So you hand that folder to DaoBox.

The files stay the files they were. You can read them like a knowledge base, and keep editing and adding. Even if you stop using DaoBox later, other editors can still open them.

**A good fit if:**

* You already have a batch of Markdown files
* You don’t want to be locked into a note app
* You want an ordinary folder to become a real knowledge base

---

## 02｜I’m just jotting things down—I don’t know what they’ll become yet

When you first capture something, you often don’t know its final purpose.

A sudden idea, a reading note, a project lesson—or materials that aren’t organized yet.

It’s too early to turn it into an “article.”

So you write it down first.

As content grows, you slowly add links, context, and structure. Loose records become a set of related knowledge.

Later—when you need an article, a doc, or a publish—you shape it from what’s already there.

**You don’t decide what it must become before you start recording.**

You accumulate first, and let it grow into shape.

---

## 03｜When I write, I keep switching between writing and reading

Sometimes you need to focus on drafting a passage.

Sometimes you’re really reading, organizing, and checking structure.

If the editor stays stuck in “you’re editing” mode, attention drifts to Markdown syntax and the cursor instead of the content.

In DaoBox, you can treat the piece as a normal document first.

When something needs changing, you edit at that spot.

When you’re done, you return to reading.

**Write when you’re writing. Read when you’re reading.**

Instead of an editor that constantly reminds you “this is a Markdown file.”

---

## 04｜I want one piece to serve both myself and others

While writing an article, you may jot down things only you need:

Why you wrote it this way, what you consulted, ideas still unverified, context for AI, or content you’re not ready to share.

If you split that out, you maintain two files.

If you delete it, you may need it later.

So leave it in the same file and mark it private.

When you read it yourself, it’s still part of the piece; when you publish, private parts don’t appear in the public output. The point is to avoid a long-lived fork between “your version” and “the published version.”

**One file can support both your own work and the final public content.**

---

## 05｜I’ve written a lot—and suddenly want it as a website

It may have started as a personal knowledge base.

One day you notice there’s enough inside:

A few articles could form a blog; a batch of notes could become a topic; long-term materials might even become a book.

You don’t need to spin up a separate “publishing project.”

You keep using the same files.

Pick a presentation style, preview the result, then publish.

What used to live only on your computer now has an entrance for other people. The product vision includes common publish shapes such as blogs and book-style knowledge bases.

**Publishing isn’t another phase—it’s a result of accumulating enough.**

---

## 06｜I’m maintaining a long-running project and need files, materials, and docs together

A long project is rarely Markdown-only.

Besides docs, there are images, PDFs, audio, video, and other project files.

If “convenient note-taking” means splitting everything into another knowledge app, materials get scattered instead.

DaoBox works better pointed at the project directory itself.

Markdown for recording and organizing; images and other materials stay where they are, and open when you need them.

So:

```text
A project
├── Docs
├── Notes
├── Images
├── PDFs
├── Other materials
└── ...
```

You don’t need a second copy detached from the project just for knowledge management.

---

## 07｜I care whether I can still find my content years from now

After years with a knowledge base, what matters most often isn’t “how fast I write today,” but whether you can still find what you wrote then.

So you want:

* Files that stay on your own computer
* History for changes
* The ability to see what a change did
* A way back to earlier versions when needed
* Syncing the repo to a remote location

DaoBox can use Git as version control for this file-based knowledge base, and keeps many operations that used to need the CLI inside the app.

The library isn’t only “what it is now”—it also keeps what it used to be.

---

## 08｜I want more and more connections among my own files

At first there are only a few notes.

Later the same idea may show up in a dozen pieces; a project may cite several background sources.

As content grows, folders alone aren’t enough.

So you start linking notes.

Jump from one piece to another, then look back at “where else is this mentioned.”

As those relationships multiply, what began as a folder gradually becomes a knowledge network that’s truly yours.

---

## 09｜I want a website without becoming a web developer first

Some people want to write publicly without first learning static site generators, the command line, Node.js, deploy configs, and the rest of the toolchain.

What they actually want is simple:

**Write content, then let people see it.**

So the site should build on content that already exists—not require you to stand up a site before you start writing.

Content remains local Markdown; publishing only adds a reader-facing presentation.

People who need deeper customization can then adjust templates and deployment.

---

## 10｜I don’t want writing and publishing to become two systems

This is where these scenarios converge.

Today you might only write a note.

Tomorrow you shape it into an article.

Months later, a few articles may form a topic.

Later still, they may become a blog, a docs site, or even a book.

From start to finish, the content doesn’t have to move.

**It’s always the same set of files.**

You’re just using them differently at different times.

That’s the habit DaoBox hopes to encourage:

```text
Capture
  ↓
Accumulate
  ↓
Organize
  ↓
Link
  ↓
Write
  ↓
Publish
```

Not every step has to happen.

Most of the time, you simply keep accumulating.

When you truly need to, you let what’s already there do more.
