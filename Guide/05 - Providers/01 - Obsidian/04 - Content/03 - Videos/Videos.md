---
status: Published
description: Embedding videos in your content.
posted on: 2026-02-27T15:36
tags: []
"[draftist] content kind": DocPage
"[draftist] content id": 019c94d8c27f795ab575faf6c5932194
"[draftist] position": 98304
"[draftist] published title": Videos
"[draftist] published slug": videos-3sili94m5
"[draftist] published on": 1779969314360
---
For now, Draftist supports only YouTube embeds. Internal video support is on the way. ^e094e0

## YouTube ^c79b3e

Embed a YouTube video using image syntax with a YouTube URL: ^ba36ae

```md
![Optional caption](https://youtu.be/VIDEO_ID)
```
^e76c8c

All common YouTube URL formats work: ^9eb0cc

- `https://youtu.be/VIDEO_ID` ^046f27
- `https://youtube.com/watch?v=VIDEO_ID` ^cfdf19
- `https://youtube.com/embed/VIDEO_ID` ^8a20e4
- `https://youtube.com/shorts/VIDEO_ID` ^039ca5
- `https://youtube.com/live/VIDEO_ID` ^64cd95

### Start Time ^5830d5

You can link to a specific timestamp using the `t` parameter (in seconds): ^6ea8c9

```md
![Caption](https://youtu.be/VIDEO_ID?t=120)
```
^a2ef9b

The `start` and `time_continue` parameters also work. ^cf5f54
