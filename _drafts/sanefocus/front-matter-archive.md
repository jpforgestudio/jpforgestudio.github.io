# Using front matter in SaneFocus notes

Front matter is a small metadata block at the top of a note. In SaneFocus, it
can keep tab names tidy and send archived text to a dedicated Markdown file.

```markdown
---
title: Inbox
archive: ~/Notes/SaneFocus/archive.md
---

- [ ] Reply to the invoice email
- [x] Check the build upload
- [c] Cancel the old follow-up
```

## Compact tab titles

Add a title when the first line of the note is not the label you want to see in
the tab strip. SaneFocus still keeps the visible tab compact, but the source of
the name becomes explicit.

## Archive finished items

Add an archive path when you want the archive shortcut to move text out of the
active note. If text is selected, that selection is moved. If nothing is
selected, completed and canceled checklist items are moved.

The archive file is plain Markdown, so it remains easy to search, back up, or
open in another editor later.

## Why this stays small

The feature is not meant to turn SaneFocus into a project manager. It is a
pressure valve for scratch notes: keep the current note light, preserve finished
context somewhere simple, and get back to work.
