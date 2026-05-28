---
status: Published
description: Platform addresses, custom domains, and DNS setup.
posted on: 2026-02-27T15:34
tags: []
"[draftist] content kind": DocPage
"[draftist] content id": 019c99d265cd726180ff75827ef0048b
"[draftist] position": 49152
"[draftist] published title": Domains
"[draftist] published slug": domains-ajx2ma539
"[draftist] published on": 1779968492132
---
Every site needs a web address. Draftist gives you one automatically, and you can add your own custom domain on top. ^3a7c6d

## Platform address ^4b8d7e

You get a platform address based on your username: ^5c9e8f

| Site | Address |
| ---- | ------- |
| Primary site | `username.draftist.io` |
| Additional sites | `username.draftist.io/~/handle` |
^6d1a9b

This works out of the box — no setup needed. ^7e2b1c

## Custom domains ^8f3c2d

You can connect a custom domain — either an apex domain (`example.com`) or a subdomain (`blog.example.com`). Add the domain in your site settings, configure the DNS records we provide at your registrar, and we verify the setup automatically. ^9a4d3e

For apex domains, you can choose between the naked version (`example.com`) and the www version (`www.example.com`), and optionally set up a redirect between the two. ^b5e4f1

## Primary address ^c6f5a2

One address serves as your site's primary — all others redirect to it. By default, that's your platform address. Once a custom domain is verified, you can switch it to primary. ^d7a6b3

---

> [!tip]
> See [Site Management > Domains](Guide/04%20-%20Site%20Management/02%20-%20Domains/Domains.md) for details on configuring your domains.
^406e4c
