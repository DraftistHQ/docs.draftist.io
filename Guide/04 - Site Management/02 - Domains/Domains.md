---
status: Draft
description: Adding custom domains, DNS setup, and managing your site's address.
posted on: ""
tags: []
"[draftist] content kind": DocPage
"[draftist] content id": 019c9a6728be7a9683a228f44918f329
"[draftist] position": 32768
"[draftist] published title": Domains
"[draftist] published slug": domains-8ljt1nos4
"[draftist] published on": 1772183255141
---
The domains page lists all addresses for your site — your platform address and any custom domains you've added. From here, you can add new domains, check verification status, and choose which address is primary. ^1f7fec

## Adding a custom domain ^50a82f

Click **Add new domain**, enter your domain (e.g., `my-site.com`), and optionally check **Make primary** to use it as your site's main address once verified. ^8f01f5

If you enter an apex domain (like `example.com`), we'll ask how you want to handle www: ^b01af6

- **example.com is the main domain** — `www.example.com` redirects to `example.com` ^d7001e
- **www.example.com is the main domain** — `example.com` redirects to `www.example.com` ^0db79e
- **example.com is the only domain** — no redirect is created ^61470d

Subdomains (like `blog.example.com`) skip this step. ^06f72a

## DNS setup ^b6c487

After adding a domain, you'll see the DNS records to configure at your registrar — typically a CNAME record pointing to our servers. ^5bc145

For apex domains where your DNS provider doesn't support CNAME at the root, we provide a backup A record as an alternative. Check the "I can't add a CNAME record for my apex domain" option to see it. ^56e546

> [!warning] 
> If you manage your DNS with Cloudflare, make sure proxying is disabled. Set the proxy status to **DNS only**.
^ac8e02

## Verification ^a5c698

Once you've configured the DNS records, verification happens automatically. You can track progress on the domain card: ^1a9e7a

- **Pending** — waiting for DNS records to be configured ^02691b
- **Verifying** — checking your DNS configuration ^22eca3
- **Verified** — ready to use ^891cb9
- **Partially verified** — main domain is verified, but the redirect record isn't yet ^fcd232
- **Failed** — verification unsuccessful; check your DNS records and try again ^493d74

You'll get an email notification when verification completes. ^f9a273

## Primary address ^f8f4d5

One address is your site's primary — all others redirect to it. Your platform address is primary by default. Click the star icon on any verified domain to make it your primary domain. ^4c7a2f

## Redirect configuration ^a9bb40

For verified apex domains, you can update the www redirect at any time using the redirect button on the domain card. ^a030e1

## Deleting a domain ^820396

Click the delete button on any custom domain to remove it. If you're deleting the primary domain, you'll be asked to pick a replacement first. ^ff04a2
