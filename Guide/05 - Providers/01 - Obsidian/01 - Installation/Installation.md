---
status: Published
description: How to install the Draftist plugin for Obsidian.
posted on: 2026-02-27T15:35
tags: []
"[draftist] content kind": DocPage
"[draftist] content id": 019c8fb1e7fb773f8b41662307169e0c
"[draftist] position": 32768
"[draftist] published title": Installation
"[draftist] published slug": installation-oc5br7o44
"[draftist] published on": 1779969141513
---
You'll need [Obsidian](https://obsidian.md) v1.11.4 or higher and a [Draftist](https://draftist.io) account. ^17c4ed

## Community Plugins (coming soon) ^2229bb

The plugin is pending approval in the Obsidian community plugins directory. ^1736cd

## BRAT (Recommended) ^b2bfdf

Since the plugin is not yet available in the community plugins directory, you can install it using [BRAT](https://github.com/TfTHacker/obsidian42-brat), a community plugin manager for [beta testing](https://docs.obsidian.md/Plugins/Releasing/Beta-testing+plugins): ^ae3089

1. Install BRAT from Obsidian's Community Plugins ^48b296
2. Open the command palette and run `BRAT: Plugins: Add a beta plugin for testing` ^828abc
3. Enter `DraftistHQ/draftist-obsidian-plugin` ^068ca1

BRAT will keep the plugin updated automatically when new versions are released. ^34b588

## Manual ^b72e77

1. Download `main.js`, `styles.css`, and `manifest.json` from the [latest release on GitHub](https://github.com/DraftistHQ/draftist-obsidian-plugin/releases/latest) ^5050fd
2. Create a `draftist` folder inside your vault's `.obsidian/plugins/` directory ^a70e05
3. Copy the downloaded files into that folder ^b1c946
4. Restart Obsidian and enable the plugin in Settings → Community Plugins ^c25d5c

With manual installation, you'll need to repeat these steps to update to newer versions. ^4fc196
