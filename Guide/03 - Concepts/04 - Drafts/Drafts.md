---
status: Published
description: The draft-first workflow — edit, preview, and go live.
posted on: 2026-02-27T15:34
tags: []
"[draftist] content kind": DocPage
"[draftist] content id": 019c99d27c17795e9e3e3f2e7c494af3
"[draftist] position": 131072
"[draftist] published title": Drafts
"[draftist] published slug": drafts-p89gllvrl
"[draftist] published on": 1781449752296
---
Content and site configuration in Draftist use a draft-first workflow. You edit a draft, preview it, and push it live when you're ready. ^e8b7c4

## Draft and Live ^f9c8d5

Every piece of content — blog posts, doc pages, etc — has two versions: **draft** and **live**. The draft is your working copy. The live version is what readers see. The two stay independent until you choose to publish. ^1a9d6e

Site configuration works the same way. You can tweak fonts, colors, and other settings in the draft without affecting your live site. ^2b1e7f

## Preview ^3c2f8d

Your draft site is always available at a separate preview address: ^4d3a9b

> [!link] username.preview.draftist.io
^5e4b1c

This shows all your latest changes — unpublished content and unpublished configuration — so you can see exactly how things look before going live. ^6f5c2d

## Content Lifecycle ^054909

After you publish something, you can still take it offline, bring it back, or delete it when you no longer need it. ^7a46bf

| State | Meaning |
| ----- | ------- |
| **Draft** | The content exists only as a draft. You can preview it, but readers can't see it. |
| **Published** | The live version is available to readers. If you edit the draft after publishing, Draftist marks it as having unpublished updates. |
| **Unpublished** | The content has been taken offline because it needs more work. The draft stays available in preview, and you can publish it again later. |
| **Archived** | The content is offline because it is no longer relevant. It is kept as archived content and can be unarchived if needed. |
| **In trash** | The content is offline and scheduled for deletion. You can restore it before the retention period ends, or delete it permanently. |
^4880cb

Publishing always promotes the current draft to a **Published** live version. ^2801b2

**Unpublished** and **Archived** publications are both offline, but they mean different things. Use **Unpublished** when something went live too soon and needs more work — it is a to-do. Use **Archived** when the content is no longer relevant and is expected to stay out of the live site. ^21a91f

## Managing Availability ^20b8e2

Use the toolbar on the preview site to manage content availability: ^6c25cb

- **Publish** — promotes the current draft to the live site. ^e42298
- **Unpublish** — removes the live version from public access, but keeps the draft. ^e09e74
- **Archive** — removes the live version from public access and marks it archived. ^7e515d
- **Unarchive** — restores archived content to the live site. ^1dda15
- **Delete** — moves content to trash. ^250949
- **Restore** — restores trashed content to its previous state. ^305511
- **Delete permanently** — removes it permanently. ^66a8ea

Trashed content is retained for 30 days before deletion. ^9d0fdf

## Link and Availability Warnings ^334503

Draftist checks links before lifecycle changes. ^cda19f

When publishing, if the draft links to content that is not published, Draftist warns you. You can publish anyway, but those links will be broken until the linked content is published. ^4e33af

When unpublishing, archiving, or deleting content, Draftist checks whether live content links to it. If so, you'll be asked to review the affected links before continuing. ^94f3ea

For doc pages, availability also depends on ancestors. If a parent page is unpublished, archived, or deleted, its published child pages become hidden from the live site until the parent is restored. ^810d4f
