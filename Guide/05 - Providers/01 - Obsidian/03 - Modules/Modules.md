---
status: Published
description: How content is organized into modules on your Draftist site.
posted on: 2026-02-27T15:35
tags: []
collapsed: true
"[draftist] content kind": DocPage
"[draftist] content id": 019c8fd598be7062a71e2cd60492b7cc
"[draftist] position": 98304
"[draftist] published title": Modules
"[draftist] published slug": modules-wqm29gbo7
"[draftist] published on": 1781450966681
---
Modules are the building blocks of your site. Each module represents a type of content — a blog, documentation, etc. You configure modules in your site settings on Draftist, giving each one a name and a URL slug. ^baeb68

> [!tip]
> See [Site Management > Modules](Guide/04%20-%20Site%20Management/03%20-%20Modules/Modules.md) for details.
^2b448a

In your vault, the folder structure mirrors this: ^9a1e0f

```
My Website/
├── Blog/
│   └── (blog posts)
└── Docs/
    └── (doc pages)
```
^561f9c

The top-level folder (`My Website`) is the site folder you chose during plugin setup. Each subfolder corresponds to a module, and its name must match the module name configured on Draftist. The content inside depends on the module kind — see the [Blog](Blog.md) and [Docs](Docs.md) pages for details. ^d2b68b
