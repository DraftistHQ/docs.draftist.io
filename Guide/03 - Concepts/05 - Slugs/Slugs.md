---
status: Draft
description: How URLs are built from your content titles.
posted on: ""
tags: []
"[draftist] content kind": DocPage
"[draftist] content id": 019c99d21f14766c9a226134969a7c79
"[draftist] position": 163840
"[draftist] published title": Slugs
"[draftist] published slug": slugs-950ltk09g
"[draftist] published on": 1772182902050
---
A slug is the URL-friendly part of a content address. Draftist generates one automatically from the title, or you can set a custom slug if you like. ^1d9a6b

## Structure ^2e1b7c

Every content slug has two parts: a **title** derived from the content title and a short **ID** that ensures uniqueness: ^3f2c8d

```
hello-world-a1b2c3d4e
            ╰── id ──╯
```
^4a3d9e

If you set a custom `slug` in the frontmatter, it replaces the auto-generated title portion. The ID is always appended. ^5b4e1f

> [!info] The ID uniquely identifies each piece of content. In the future, you'll be able to use it as a short link — e.g. `your-site.com/a1b2c3d4e` — to share content.
^19bbe2

## URL paths ^6c5f2a

The full URL combines the [module](Guide/03%20-%20Concepts/03%20-%20Modules/Modules.md) slug with the content slug. ^7d6a3b

Blog posts: ^8e7b4c

```
/blog/hello-world-a1b2c3d4e
```
^9f8c5d

Doc pages include their ancestor path: ^a1d9e6

```
/docs/getting-started/installation-b2e1f7c8a
```
^b2e1f7

## Redirects ^c3f2a8

If a title changes and the slug updates as a result, old URLs redirect to the new one automatically — existing links won't break. ^d4a3b9
