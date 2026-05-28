---
status: Published
description: Building structured documentation sites with the Obsidian plugin.
posted on: 2026-02-27T15:35
tags: []
"[draftist] content kind": DocPage
"[draftist] content id": 019c9464add5765f97653f77cd5a00f5
"[draftist] position": 65536
"[draftist] published title": Docs
"[draftist] published slug": docs-kbfv0qdbc
"[draftist] published on": 1779969222751
---
> [!warning]
> The Docs module is currently in private beta.
^477482

The Docs module is for structured content — guides, references, tutorials, or even a whole book. Pages are organized in a tree that maps directly to your folder structure. The site you're reading right now is built with it. ^9606dc

## Anatomy of a Doc Page ^9d4ade

- **Title**
  The filename of the note. You'll be asked for it when creating a page via the plugin commands. ^6c4553
- **Description**
  A short summary set in the `description` field of the frontmatter. It shows up in search engine results and social media previews. Don't skip it! ^5c88fe
- **Body**
  Everything below the frontmatter. See the Content section for formatting, images, code blocks, and other supported elements. ^d591ff

## Page Lifecycle ^c7afbd

Every page has a `status` in its frontmatter: ^47d111

- **Draft** — work in progress, can be previewed on your site but not visible to readers. ^671658
- **Published** — live on your site. ^f7ebe1
- **Archived** — removed from public view. ^06729a

## Folder Structure ^f762d4

Folder nesting defines the page hierarchy, and numeric prefixes reflect ordering. Each folder follows the `NN - Title` pattern — the prefix sets the position in the file tree. These only exist to keep things sorted in Obsidian's file explorer; the actual order on your site is tracked separately. The plugin assigns prefixes automatically when you create pages, so you don't need to worry about them. ^94fb62

There are two kinds of entries: **pages** and **groups**. A page has content. A group is a section label that organizes child pages — it shows up in the sidebar but doesn't have its own page (though it might). To make a group, just leave the note's body empty. A page with children works too — it serves as both a section and a standalone page. ^5242ad

```
My Website/
└── Docs/
    ├── 01 - Getting Started/
    │   ├── Getting Started.md
    │   ├── 01 - Installation/
    │   │   └── Installation.md
    │   └── 02 - Configuration/
    │       └── Configuration.md
    ├── 02 - Guides/
    │   ├── Guides.md
    │   └── 01 - Writing Content/
    │       └── Writing Content.md
    └── 03 - Reference/
        └── Reference.md
```
^cfcfb8

The `Docs` folder name must match the module name in your site settings. ^70f012

Each page lives in its own folder — the markdown file and all its assets are kept together: ^ac663c

```
01 - Getting Started/
├── Getting Started.md
└── images/
    ├── doc-screenshot.a1b2c3d4.png
    └── ...
```
^db82a3

> [!info]
> When you rename a page file, the plugin automatically renames its folder to match. When you delete a page folder, sibling folders are automatically renumbered to keep the sequence clean.
^1b9005

## Creating a Page ^fa00cf

Open the command palette (`Ctrl/Cmd + P`) and run `Draftist: Create new doc page`. Pick a location in the tree, enter a title and description, and the plugin creates the folder with the correct prefix and a note with pre-filled frontmatter. ^a784f6

You can also right-click a folder in the file explorer and use either "Add page before", "Add page after", or "Add child page". ^48b532

### Adding Images ^108349

- **Inline images** — embed images directly in your page body. See [Images](Guide/05%20-%20Providers/01%20-%20Obsidian/04%20-%20Content/02%20-%20Images/Images.md) for details. ^8707c1
- **Galleries** — display a collection of images in a grid layout. See [Galleries](Guide/05%20-%20Providers/01%20-%20Obsidian/04%20-%20Content/02%20-%20Images/Images.md#^54b1c5) for details. ^9f3440

All images are stored in the page's `images/` subfolder — the plugin handles this automatically when you add assets via the provided commands. If you've added images manually or they ended up outside the `images/` folder, run `Draftist: Normalize images` to reorganize them into the correct location with consistent filenames. ^1ce142

## Frontmatter ^0b180b

Here are the frontmatter fields the plugin manages: ^316bbb

| Field         | Description                                                                 |
| ------------- | --------------------------------------------------------------------------- |
| `status`      | Page lifecycle stage: `Draft`, `Published`, or `Archived`                   |
| `description` | Short summary shown in SEO meta tags                                        |
| `posted on`   | Publication date (`YYYY-MM-DD`). Auto-assigned on first publish if not set. |
| `slug`        | Custom URL slug. Auto-generated from the title if not set.                  |
| `tags`        | List of tags                                                                |
| `collapsed`   | When set to `true`, the page's children are collapsed in the sidebar by default |
^d7390d

> [!tip]
> If you created a note manually or its frontmatter looks out of order, run `Draftist: Normalize frontmatter`. It sorts all properties into a consistent order and adds any missing fields.
^177ecf

> [!warning]
> The plugin also stores internal metadata in fields prefixed with `[draftist]`. These are hidden by default — you'll only see them if you enable "Expose internal metadata" in the plugin's debugging settings. Don't edit them manually — changing these values can corrupt the plugin's sync state and cause publishing issues.
^02f8b4

## Publishing ^8d60dc

When you're ready, run [`Draftist: Preview and publish` command](Commands.md#^32ee3c). The plugin saves a draft version of your page and opens it in your browser on your site's preview domain so you can check it out before making it public. ^5a7633

> [!warning]
> If you use other third-party Obsidian plugins, the Obsidian team [recommends](https://help.obsidian.md/plugins/web-viewer#Security) using your primary browser for sensitive tasks and websites that require login instead of the web viewer for security reasons.
^08b2cc

> [!info]
> During publishing, the plugin adds block ID markers (like `^a1b2c3`) to every block in your page. We know they can be a bit noisy, but they power useful features: readers and other pages can link directly to a specific paragraph or heading, they enable automatic table of contents generation, and the server can diff changes between versions to show exactly what was updated. You can adjust their opacity or disable them entirely in the plugin settings — though we recommend keeping them on.
^ad0b92

Parent pages must be published before their children — the plugin will let you know if you try to publish a child whose parent isn't live yet. We'll make this one easier in the future. ^2460b3

After publishing, when you return to the note, the plugin syncs the page's status and publication date back from your site. ^9b2377
