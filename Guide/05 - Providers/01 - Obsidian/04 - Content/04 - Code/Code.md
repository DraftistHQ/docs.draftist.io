---
status: Published
description: Syntax-highlighted code blocks with filenames, line highlighting, and captions.
posted on: 2026-02-27T15:36
tags: []
"[draftist] content kind": DocPage
"[draftist] content id": 019c94ef4f457aa0bec98d222cf4225a
"[draftist] position": 131072
"[draftist] published title": Code
"[draftist] published slug": code-hz8xug3dc
"[draftist] published on": 1781451036627
---
Use fenced code blocks with a language identifier for syntax highlighting: ^c1ec01

````md
```rust
fn main() {
    println!("Hello!");
}
```
````
^09a10c

Renders as: ^fde9e1

```rust
fn main() {
    println!("Hello!");
}
```
^dc7be0

## Supported Languages ^2c6330

Syntax highlighting is powered by PrismJS. We're still expanding the set of supported languages — if yours isn't highlighted yet, it will be soon. ^e96c26

> [!tip]
> Ping us on [Discord](https://discord.gg/nZhbzzbT5A) if the language you need is missing!
^bf95d5

## Meta Attributes ^b53a1f

You can add attributes after the language identifier to control how the block looks. Use `key=value` syntax, separated by spaces: ^458b97

| Attribute   | Description                          | Example                              |
| ----------- | ------------------------------------ | ------------------------------------ |
| `file`      | Display a filename badge             | `file=parser.rs`                     |
| `highlight` | Highlight specific lines             | `highlight=3,5-8,12`                |
| `caption`   | Add a description below the block    | `caption="Error handling logic"`     |
^57d2a3

### Filename ^a97f2d

Shows a filename badge in the code block header: ^3eacfe

````md
```rust file=src/main.rs
fn main() {
    let config = Config::load();
    run(config);
}
```
````
^8a0478

Renders as: ^759f93

```rust file=src/main.rs
fn main() {
    let config = Config::load();
    run(config);
}
```
^72b19a

### Line Highlighting ^6aa4f4

Highlight specific lines to draw attention to important parts: ^2a515b

````md
```python highlight=3-4
def greet(name):
    """Say hello."""
    message = f"Hello, {name}!"
    print(message)
```
````
^2eab69

Renders as: ^eb20f7

```python highlight=3-4
def greet(name):
    """Say hello."""
    message = f"Hello, {name}!"
    print(message)
```
^d12346

| Format | Example | Description |
| ------ | ------- | ----------- |
| Single line | `highlight=5` | Highlights line 5 |
| Range | `highlight=10-15` | Highlights lines 10 through 15 |
| Mixed | `highlight=2,5-8,12` | Combines singles and ranges |
^ad4c87

### Caption ^616c74

Captions show up below the code block: ^639840

````md
```javascript file=api.js highlight=4 caption="User fetching and parsing"
async function fetchUser(id) {
    const response = await fetch("/api/users/" + id);
    const data = await response.json();
    return User.parse(data);
}
```
````
^61a025

Renders as: ^0625c3

```javascript file=api.js highlight=4 caption="User fetching and parsing"
async function fetchUser(id) {
    const response = await fetch("/api/users/" + id);
    const data = await response.json();
    return User.parse(data);
}
```
^d09618

## UI Features ^e84270

Every code block comes with a **copy button** and a **language badge**. If the block has a block ID, there's also a **link button** so readers can grab a direct link to it. ^8b060c
