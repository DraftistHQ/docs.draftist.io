---
status: Published
description: Embedding images, controlling layout, and creating galleries.
posted on: 2026-02-27T15:35
tags: []
"[draftist] content kind": DocPage
"[draftist] content id": 019c94d1a439795dba036d947ef606da
"[draftist] position": 65536
"[draftist] published title": Images
"[draftist] published slug": images-0efwwejjn
"[draftist] published on": 1781451017401
---
The easiest way to add images is with the `Draftist: Insert image` command. Pick an image, set a caption and placement, and the plugin copies it to the right spot with a clean filename. The result is standard Markdown: ^0ca026

```md
![Optional caption text](images/post-photo.a1b2c3d4.jpg)
```
^1166c1

The alt text becomes the image caption on your site. ^738b74

![Sheikh Zayed Grand Mosque](doc-post-DSC00502-Edit-Edit.d9f883e9.027e7b58.jpg) ^17e6cf

## Placement ^67cc38

Most of the time, you don't need to worry about placement — the defaults look good. But when you want more control: ^1baebd

| Placement | Behavior |
| --------- | -------- |
| `wide`    | Extends beyond the text column on larger screens |
| `fit`     | Fills the text column width |
| `narrow`  | Narrower than the text column |
^db32c3

> [!info]
> Landscape images default to `fit` and portrait images default to `narrow`.
^60e236

Set placement in the title attribute: ^2e5d5b

```md
![Caption](image.jpg "placement=wide")
```
^a25cc1

To set both a title and placement, separate them with `|||`: ^c98f46

```md
![Caption](image.jpg "Morning view ||| placement=wide")
```
^f17814

## External Images ^5bd94a

You can use external URLs instead of vault images: ^3cddff

```md
![Caption](https://example.com/photo.jpg)
```
^d5a910

> [!warning]
> We strongly recommend using vault images. External ones are rendered as-is with no processing — their dimensions are unknown, so they can break your layout, cause content to jump around as they load, and won't get placeholders or size optimization. They can also disappear if the source goes down.
^3dc387

## Galleries ^54b1c5

Want to show multiple images together? Use the `Draftist: Insert gallery` command — pick your images, add an optional caption, and the plugin handles the rest. It uses the `[!GALLERY]` callout syntax: ^36cc39

```md
> [!GALLERY] Optional caption
> ![First image caption](image1.jpg)
> ![Second image caption](image2.jpg)
> ![](image3.jpg)
```
^6833d5

Each image can have its own caption (via alt text) and title. ^918b2d

> [!GALLERY]- Turkey
> ![](doc-post-DSC02640.f456e500.13fee362.jpg)
> ![](doc-post-DSC02554.b6346bb6.0b14300a.jpg)
> ![](doc-post-DSC02771-Edit.aacbd1ac.24a1b2c1.jpg)
> ![](doc-post-DSC03210.72b567b3.4fadd7e6.jpg)
> ![](doc-post-DSC02801.310fe3ef.2ec46adb.jpg)
> ![](doc-post-DSC03443.6d6d5352.76a004f8.jpg)
> ![](doc-post-DSC03536.d520b19f.c5a48a5b.jpg)
^b89de1

## Optimizations ^3f3777

Vault images are automatically optimized when published: they're served in multiple sizes for different viewports, lazy-loaded as you scroll, and displayed with state-of-the-art placeholders while loading. ^06d716

## Supported Formats ^30c869

**Allowed formats:** JPG, PNG, WebP, GIF
**Maximum file size:** 10 MB ^19a894
