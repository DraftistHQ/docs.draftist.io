---
status: Published
description: Plugin settings and what they do.
posted on: 2026-02-27T15:36
tags: []
"[draftist] content kind": DocPage
"[draftist] content id": 019c9f11035e76afa924787030c5bf8d
"[draftist] position": 147456
"[draftist] published title": Settings
"[draftist] published slug": settings-uk45m1cnu
"[draftist] published on": 1781451067234
---
The Draftist plugin settings are accessible through Obsidian's Settings → Community Plugins → Draftist. Settings are organized into several sections. ^836a1d

## Authentication ^8884f9

- **Token** — your Draftist API token, stored securely in Obsidian's secret storage. ^afc3d7

> [!info]
> Manage API tokens at [Draftist](https://draftist.io/manage/account/security/tokens).
^5edf9b

## Sites ^767ab4

Lists all sites associated with your account. For each site, you can: ^6ea3ad

- **Set a folder path** — the vault folder where the site's content lives. ^19e7bd
- **Enable or disable** — toggle whether the plugin manages a particular site in the current vault. ^8e75f3

> [!tip]
> If your vault is dedicated to a single site, you can set `/` as the folder path to use the vault root directly instead of creating a subfolder.
^6aef28

Use **Refresh sites** to pull the latest site list from Draftist if you've made changes on the web. ^072132

## Automations ^0feb78

- **Manage site folders** — automatically creates and organizes the file and folder structure for your sites. ^264dca

> [!warning]
> We strongly recommend keeping this enabled, as manual management currently might have some rough edges. Managing site folders manually is possible, but not well tested, so it's error-prone.
^4b9f29

## Block IDs ^475cea

Block IDs are short identifiers appended to content blocks (paragraphs, headings, list items, etc.) that make individual blocks linkable. When enabled, the plugin automatically generates and manages them — you don't need to add or edit them yourself. ^04c9e2

Block IDs enable several features: ^a3829b

- **Deep linking** — link not just to a page but to a specific paragraph, heading, or list item within it. You can cross-link from your content. Your site visitors can do this too! ^e5199a
- **Table of contents** — headings with block IDs power automatic TOC generation for your content. ^c11529
- **Content diffing** — block IDs let the system track individual blocks across edits. In the future, we will allow tracking content changes, so users will be able to see exactly what changed in the recent update. ^940dd0

During publishing, the plugin checks that linked blocks exist, so you'll catch broken references before they go live. ^0b4578

We strongly recommend keeping it on. Without them, you lose all these goodies. ^0fe58c

- **Enable** — toggles block ID generation. Enabled by default. Disabling won't remove existing IDs, but new blocks won't get them. ^3e0359
- **Opacity** — controls how visible block IDs are in the editor. Defaults to very subtle so they stay out of your way while writing. ^52e604

## Debugging ^dc7a68

- **Extensive logging** — enables detailed logging for troubleshooting. ^344f5f
- **Expose internal metadata** — makes internal frontmatter fields visible in the editor. ^119e82

These are off by default and only useful when diagnosing issues. ^ca5e1b
