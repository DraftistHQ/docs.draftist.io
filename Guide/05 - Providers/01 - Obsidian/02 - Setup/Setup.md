---
status: Published
description: Connect the Draftist plugin to your account and configure your vault.
posted on: 2026-02-27T15:35
tags: []
"[draftist] content kind": DocPage
"[draftist] content id": 019c8fcd8eae7f9d8c06facebea0f9dd
"[draftist] position": 65536
"[draftist] published title": Setup
"[draftist] published slug": setup-tgr6qth85
"[draftist] published on": 1781450956163
---
After installing the plugin, open its settings in Obsidian (Settings → Draftist). You'll see a setup wizard that walks you through the initial configuration. ^0c85f4

## Add Auth Token ^60976d

1. In the setup wizard, click "Get Started". ^cbf0a6
2. On the API Token step, click "Get token" — this opens the Draftist page where you can copy your token. ^2ac435
3. Back in Obsidian, click "Link..." to create an Obsidian secret and paste your token. You can name the secret anything you like (e.g., "Draftist Token") — it's just a label to identify it among your other Obsidian secrets. ^187330
4. Click "Next" — the plugin will verify your token and fetch your sites. ^af3b85

> [!INFO]
> Your token is stored in Obsidian's secure secret storage, not in plain text.
^262515

## Configure Sites ^2d2bc9

Next, the wizard will show your Draftist sites. For each site you want to manage from this vault: ^788ec0

1. Enter a **folder path** — this is where your site's content will live in the vault (e.g., `My Website`). The folder will be created if it doesn't exist. ^31491d
2. If you have multiple sites, uncheck any you don't want to manage in this vault. ^53f345

Click "Finish" to complete the setup. The plugin will create the folder structure for your sites, and you're ready to start writing. ^86970c
