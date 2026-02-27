---
status: Draft
description: How content is organized into modules on your Draft42 site.
posted on: ""
tags: []
collapsed: true
"[d42] content kind": DocPage
"[d42] content id": 019c8fd598be7062a71e2cd60492b7cc
"[d42] position": 98304
"[d42] published title": Modules
"[d42] published slug": modules-wqm29gbo7
"[d42] published on": 1772192145395
---
Modules are the building blocks of your site. Each module represents a type of content — a blog, documentation, etc. You configure modules in your site settings on Draft42, giving each one a name and a URL slug. ^baeb68

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

The top-level folder (`My Website`) is the site folder you chose during plugin setup. Each subfolder corresponds to a module, and its name must match the module name configured on Draft42. The content inside depends on the module kind — see the [Blog](Blog.md) and [Docs](Docs.md) pages for details. ^d2b68b
