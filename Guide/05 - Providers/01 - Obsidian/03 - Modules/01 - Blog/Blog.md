---
status: Published
description: Writing and managing blog posts with the Obsidian plugin.
posted on: 2026-02-27T15:35
tags: []
"[draftist] content kind": DocPage
"[draftist] content id": 019c93e2ad2e763eb8eae5c8d3d01a2e
"[draftist] position": 32768
"[draftist] published title": Blog
"[draftist] published slug": blog-20z7s2jqr
"[draftist] published on": 1779969173413
---
The Blog module is your date-sorted feed — articles, updates, announcements, whatever you want to share. ^9f828f

## Anatomy of a Blog Post ^d1bac7

- **Title**
  The filename of the note. You'll be asked for it when creating a post via the plugin commands. ^4ba507
- **Description**
  A short summary set in the `description` field of the frontmatter. It doesn't appear in the post body itself, but it shows up everywhere else: in the list of posts on your site, in search engine results, and in social media previews when someone shares your link. A good description makes your publication look polished and helps readers decide whether to click through — don't skip it! ^9d1ac8
- **Cover**
  An optional image is displayed at the top of the post, in post listings, and used as an OG image. Can be a vault image or an external URL. Although we highly recommend using internal images. Use [`Draftist: Set cover image` command](Commands.md#^ae2d61) to set it, with optional credit text and link for attribution. ^86d3cf
- **Body**
  Everything below the frontmatter. See the [Content](Content.md) section for formatting, images, code blocks, and other supported elements. ^e51e7e

## Post Lifecycle ^d784e1

Every post has a `status` in its frontmatter that controls where it lives and whether it's public: ^7955e9

- **Idea** — early stage, not publishable ^c458dd
- **Draft** — work in progress, can be previewed on your site but not visible to readers ^0fc058
- **Published** — live on your site ^e6395b
- **Archived** — removed from public view ^bcdec4

To move a post between stages, just change the `status` field. The plugin automatically moves the file to the matching folder. ^4c5dc9

> [!info]
> Only **Published** and **Archived** statuses affect your site. Idea and Draft are just organizational labels for your writing process — treat them as suggestions. You can start everything as a Draft and ignore Ideas entirely if that suits your workflow. If there's demand, we're open to making pre-published statuses configurable so you can define your own.
^eba585

## Folder Structure ^8e840e

With the "Manage site folders" automation enabled, the plugin organizes posts by status: ^dbd5c8

```
My Website/
└── Blog/
    ├── Ideas/
    │   └── Post Title/
    ├── Drafts/
    │   └── Post Title/
    ├── Published/
    │   └── 2025-12-19 - Post Title/
    └── Archive/
        └── 2025-06-01 - Post Title/
```
^78af08

Posts with a `posted on` date get a date prefix in their folder name so they sort nicely. The `Blog` folder name matches the module name in your site settings. ^006bc0

Each post lives in its own folder — the markdown file and all its assets are kept together: ^7f822e

```
Post Title/
├── Post Title.md
└── images/
    ├── cover-hero.a1b2c3d4.jpg
    ├── post-diagram.e5f6g7h8.png
    └── ...
```
^7dbb85

## Creating a Post ^0944f5

Open the command palette (`Ctrl/Cmd + P`) and run one of: ^f06edb

- `Draftist: Create new blog post idea` — creates a post with `Idea` status ^e6fde4
- `Draftist: Create new blog post draft` — creates a post with `Draft` status ^8ad7e3

The plugin asks for a title and description, then creates a note with pre-filled frontmatter. ^ecf348

### Adding Images ^8f9413

- **Cover image** — run `Draftist: Set cover image` to pick a vault image or paste an external URL. You can optionally add credit text and a link for attribution. The cover appears at the top of the post, in post listings, and is used as an OG image. ^adbffc
- **Inline images** — embed images directly in your post body. See [Images](Guide/05%20-%20Providers/01%20-%20Obsidian/04%20-%20Content/02%20-%20Images/Images.md) for details. ^4d2c07
- **Galleries** — display a collection of images in a grid layout. See [Galleries](Guide/05%20-%20Providers/01%20-%20Obsidian/04%20-%20Content/02%20-%20Images/Images.md#^54b1c5) for details. ^5bcf7f

All images are stored in the post's `images/` subfolder — the plugin handles this automatically when you add assets via the provided commands. If you've added images manually or they ended up outside the `images/` folder, run [`Draftist: Normalize images` command](Commands.md#^70f98b) to reorganize them into the correct location with consistent filenames. ^7d959f

## Frontmatter ^b0809b

Here are the frontmatter fields the plugin manages: ^5a79f9

| Field               | Description                                                                 |
| ------------------- | --------------------------------------------------------------------------- |
| `status`            | Post lifecycle stage: `Idea`, `Draft`, `Published`, or `Archived`           |
| `description`       | Short excerpt shown in post listings and SEO meta tags                      |
| `posted on`         | Publication date (`YYYY-MM-DD`). Auto-assigned on first publish if not set. |
| `cover`             | Cover image filename or external URL                                        |
| `cover credit text` | Attribution text for the cover image                                        |
| `cover credit link` | Attribution link for the cover image                                        |
| `slug`              | Custom URL slug. Auto-generated from the title if not set.                  |
| `tags`              | List of tags                                                                |
^973a1f

> [!tip]
> If you created a note manually or its frontmatter looks out of order, run `Draftist: Normalize frontmatter`. It sorts all properties into a consistent order and adds any missing fields.
^5ba19d

> [!warning]
> The plugin also stores internal metadata in fields prefixed with `[draftist]`. These are hidden by default — you'll only see them if you enable "Expose internal metadata" in the plugin's debugging settings. Don't edit them manually — changing these values can corrupt the plugin's sync state and cause publishing issues.
^c9dda9

## Publishing ^01f896

When you're ready, run [`Draftist: Preview and publish` command](Commands.md#^32ee3c). The plugin saves a draft version of your post and opens it in your browser on your site's preview domain so you can check it out before making it public. ^c1d874

> [!warning]
> If you use other third-party Obsidian plugins, the Obsidian team [recommends](https://help.obsidian.md/plugins/web-viewer#Security) using your primary browser for sensitive tasks and websites that require login instead of the web viewer for security reasons.
^46f9a3

> [!info]
> During publishing, the plugin adds block ID markers (like `^a1b2c3`) to every block in your post. We know they can be a bit noisy, but they power useful features: readers and other posts can link directly to a specific paragraph or heading, they enable automatic table of contents generation, and the server can diff changes between versions to show exactly what was updated. You can adjust their opacity or disable them entirely in the plugin settings — though we recommend keeping them on.
^55b563

After publishing, when you return to the note, the plugin syncs the post's status and publication date back from your site. If you published a Draft, the `status` field updates to `Published` and a `posted on` date is filled in if it wasn't already set — which also triggers the folder automation, moving your post from `Drafts/` to `Published/`. ^d48119
