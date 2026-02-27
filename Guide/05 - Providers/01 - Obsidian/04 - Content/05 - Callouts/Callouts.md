---
status: Draft
description: Callouts for highlighting important information, and blockquotes for quotations.
posted on: ""
tags: []
"[d42] content kind": DocPage
"[d42] content id": 019c9521d2be77caa1feec2046bed8e2
"[d42] position": 163840
"[d42] published title": Callouts
"[d42] published slug": callouts-52ak954te
"[d42] published on": 1772193301142
---
Callouts are colored boxes that highlight important information. Blockquotes are for quotations. ^89afdc

## Callout Types ^ce0255

Use `> [!TYPE]` to create a callout: ^31d007

```md
> [!warning]
> Something to watch out for.
```
^227c5b

Renders as: ^1f7799

> [!warning]
> Something to watch out for.
^4044aa

Here are all the types you can use: ^8424d4

| Type | Aliases | Purpose |
| ---- | ------- | ------- |
| `note` | | General supplementary information |
| `info` | | Informational emphasis |
| `tip` | `hint`, `important` | Helpful advice and best practices |
| `link` | | Related resources or references |
| `question` | `help`, `faq` | FAQs or prompts for consideration |
| `warning` | `caution`, `attention` | Something to watch out for |
| `danger` | `error` | Critical issues requiring attention |
| `failure` | `fail`, `missing` | Errors or unsuccessful operations |
| `success` | `check`, `done` | Positive outcomes or completed tasks |
| `example` | | Concrete examples |
^32de4b

> [!note]
> General information that supplements the main text.
^952991

> [!info]
> Similar to note, but emphasizes informational content.
^3d8b85

> [!tip]
> Helpful advice or best practices.
^612040

> [!link]
> Highlight related resources or external references.
^4e21c8

> [!question]
> FAQs or prompts for consideration.
^fd7f29

> [!warning]
> Something to watch out for.
^aa9e49

> [!danger]
> Critical issues requiring immediate attention.
^686cce

> [!failure]
> Errors or unsuccessful operations.
^4b92f2

> [!success]
> Positive outcomes or completed tasks.
^2457a4

> [!example]
> Concrete examples or code snippets.
^4dee9a

Type names are case-insensitive — `[!WARNING]`, `[!Warning]`, and `[!warning]` all work. ^e28672

## Custom Titles ^a22dd9

Add a title after the type: ^a2972c

```md
> [!warning] Breaking Change
> This API will change in version 2.0.
```
^d52a0b

Renders as: ^5543bb

> [!warning] Breaking Change
> This API will change in version 2.0.
^1f25d9

## Collapsible Callouts ^43c14b

Add `-` (collapsed by default) or `+` (expanded by default) after the type to make a callout collapsible: ^067231

```md
> [!note]- Collapsed by default
> Hidden until you click the header.
```
^cc75d6

Renders as: ^867e6e

> [!note]- Collapsed by default
> Hidden until you click the header.
^28d86a

```md
> [!tip]+ Expanded by default
> Starts open but can be collapsed.
```
^e9e890

Renders as: ^505bc6

> [!tip]+ Expanded by default
> Starts open but can be collapsed.
^d53b5a

Without a suffix, the callout is always visible and not collapsible. ^c7d57f

## Rich Content ^88570b

You can put almost anything inside a callout — paragraphs, lists, code blocks, images, you name it: ^474826

```md
> [!example] Mixed Content
>
> Here's a paragraph explaining the concept.
>
> A list of requirements:
> - Rust 1.70+
> - Basic Rust knowledge
>
> And some code:
> ```rust
> let x = 42;
> ```
```
^2f7539

Renders as: ^965531

> [!example] Mixed Content
>
> Here's a paragraph explaining the concept.
>
> A list of requirements:
> - Rust 1.70+
> - Basic Rust knowledge
>
> And some code:
> ```rust
> let x = 42;
> ```
^ca5d14

## Blockquotes ^1034ab

Regular markdown blockquotes render as quotations: ^a77360

```md
> Design is not just what it looks like and feels like.
> Design is how it works.
```
^668dc1

Renders as: ^328930

> Design is not just what it looks like and feels like.
> Design is how it works.
^a1f016

Add attribution with `--` on the last line: ^557924

```md
> Any fool can write code that a computer can understand.
> Good programmers write code that humans can understand.
>
> -- Martin Fowler
```
^4ab8d0

Renders as: ^d820d7

> Any fool can write code that a computer can understand.
> Good programmers write code that humans can understand.
>
> -- Martin Fowler
^dcd02f
