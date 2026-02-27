---
status: Draft
description: How to install the Draft42 plugin for Obsidian.
posted on: ""
tags: []
"[d42] content kind": DocPage
"[d42] content id": 019c8fb1e7fb773f8b41662307169e0c
"[d42] position": 32768
"[d42] published title": Installation
"[d42] published slug": installation-oc5br7o44
"[d42] published on": 1772189531429
---
You'll need [Obsidian](https://obsidian.md) v1.11.4 or higher and a [Draft42](https://draft42.io) account. ^17c4ed

## Community Plugins (coming soon) ^2229bb

The plugin is pending approval in the Obsidian community plugins directory. ^1736cd

## BRAT (Recommended) ^b2bfdf

Since the plugin is not yet available in the community plugins directory, you can install it using [BRAT](https://github.com/TfTHacker/obsidian42-brat), a community plugin manager for [beta testing](https://docs.obsidian.md/Plugins/Releasing/Beta-testing+plugins): ^ae3089

1. Install BRAT from Obsidian's Community Plugins ^48b296
2. Open the command palette and run `BRAT: Plugins: Add a beta plugin for testing` ^828abc
3. Enter `Draft42HQ/draft42-obsidian-plugin` ^068ca1

BRAT will keep the plugin updated automatically when new versions are released. ^34b588

## Manual ^b72e77

1. Download `main.js`, `styles.css`, and `manifest.json` from the [latest release on GitHub](https://github.com/Draft42HQ/draft42-obsidian-plugin/releases/latest) ^5050fd
2. Create a `draft42` folder inside your vault's `.obsidian/plugins/` directory ^a70e05
3. Copy the downloaded files into that folder ^b1c946
4. Restart Obsidian and enable the plugin in Settings → Community Plugins ^c25d5c

With manual installation, you'll need to repeat these steps to update to newer versions. ^4fc196
