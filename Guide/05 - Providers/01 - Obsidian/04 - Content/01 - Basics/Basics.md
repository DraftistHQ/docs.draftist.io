---
status: Draft
description: Headings, paragraphs, lists, inline formatting, links, and more.
posted on: ""
tags: []
"[draftist] content kind": DocPage
"[draftist] content id": 019c94839fe27db6bad7a6533540f076
"[draftist] position": 32768
"[draftist] published title": Basics
"[draftist] published slug": basics-t15baju8k
"[draftist] published on": 1772192554221
---
All the standard Markdown you know and love works out of the box. Here's a quick rundown. ^f1cc95

## Headings ^a2bdb6

Use `##` through `######` for levels 2–6. H1 is reserved for the page title, so start at H2. On doc pages, headings automatically generate the table of contents. ^9ddb77

## Paragraphs ^237d65

Plain text separated by blank lines — nothing special here. ^25f430

## Inline Formatting ^af3414

- `**bold**` — **bold** ^c15c15
- `_italic_` — _italic_ ^4e7979
- `~~strikethrough~~` — ~~strikethrough~~ ^2b15ec
- `` `inline code` `` — `inline code` ^18f5be

You can nest these too: `**_bold italic_**` → **_bold italic_**. ^afe20f

## Links ^b5bd4a

### External Links ^e18be1

Standard Markdown links — nothing fancy: ^c2c055

```md
[Draftist](https://draftist.io)
```
^293cc3

### Internal Links ^a1c952

Link to other pages on your site using the same standard Markdown: ^0ba30b

```md
[Link text](Page Title)
[Deep link text](Page Title#^block-id)
```
^4932c4

> [!warning]
> Draftist requires standard Markdown links, not `[[wiki-link]]` syntax. Make sure "Use \[\[Wikilinks\]\]" is turned off in Obsidian's settings (Settings → Files and links).
^8ab0f8

The plugin resolves internal links during publishing and checks that target pages exist. Deep links (using `#^block-id`) point straight to a specific element on the page. ^20e84e

## Lists ^592a06

### Unordered Lists ^7e0ac8

```md
- First item
- Second item
  - Nested item
```
^f96f93

### Ordered Lists ^3b0e3f

```md
1. First item
2. Second item
   1. Nested item
```
^6545e1

Ordered lists support custom start numbers. You can mix ordered and unordered when nesting, and go as deep as you like. ^514f06

## Horizontal Rules ^064a5a

Drop `---`, `***`, or `___` on its own line for a thematic break between sections. ^126396
