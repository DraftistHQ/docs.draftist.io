---
status: Draft
description: GFM-style tables with column alignment.
posted on: ""
tags: []
"[draftist] content kind": DocPage
"[draftist] content id": 019c952db40c7372a28446c5ac5b5090
"[draftist] position": 196608
"[draftist] published title": Tables
"[draftist] published slug": tables-htjalgwh6
"[draftist] published on": 1772193328180
---
Standard GFM (GitHub Flavored Markdown) tables work out of the box: ^c021b7

```md
| Name   | Role     |
| ------ | -------- |
| Alice  | Engineer |
| Bob    | Designer |
```
^07a337

Renders as: ^655136

| Name   | Role     |
| ------ | -------- |
| Alice  | Engineer |
| Bob    | Designer |
^87e5de

## Column Alignment ^b2eadd

Use colons in the separator row to control text alignment: ^de1222

```md
| Left   | Center | Right |
| :----- | :----: | ----: |
| Alice  | 42     | $100  |
| Bob    | 17     | $250  |
```
^447903

Renders as: ^23a4d7

| Left   | Center | Right |
| :----- | :----: | ----: |
| Alice  | 42     | $100  |
| Bob    | 17     | $250  |
^af27cf

| Syntax | Alignment |
| ------ | --------- |
| `:---` | Left |
| `:---:` | Center |
| `---:` | Right |
| `---` | Default (left) |
^112ab9

## Inline Formatting ^48430a

Cells support all the usual inline formatting — **bold**, _italic_, ~~strikethrough~~, `inline code`, and [links](https://draftist.io): ^be88c8

```md
| Feature      | Status          |
| ------------ | --------------- |
| **Images**   | `Supported`     |
| _Videos_     | ~~Coming soon~~ |
```
^52eb0b

Renders as: ^98de3d

| Feature      | Status          |
| ------------ | --------------- |
| **Images**   | `Supported`     |
| _Videos_     | ~~Coming soon~~ |
^4cac8b
