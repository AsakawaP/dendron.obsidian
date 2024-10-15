# dendron.obsidian

> There is no loftier ambition than the pursuit of knowledge.

## TL;DR

This project aims to explore a workflow to integrate the strengths of [Dendron][] and [Obsidian][] both :-)

[Dendron]: https://www.dendron.so
[Obsidian]: https://obsidian.md

---

- [TL;DR](#tldr)
- [Features](#features)
- [How to Use](#how-to-use)
- [File Structure](#file-structure)
  - [VSCode and Git](#vscode-and-git)
  - [Dendron](#dendron)
  - [Obsidian](#obsidian)

---

## Features

- Plain text  
  Managing with Git
- Hierarchies notes  
  Designed by Dendron
- Cross-platform  
  Exploring notes with Obsidian app

## How to Use

Open this repository with Dendron or Obsidian, explore Markdown files in `notes` directory.

## File Structure

```plain-text
dendron.obsidian/
├── notes/
├── dependencies/
│   ├── localhost/
│   │   └── vault.local/
│   └── github.com/
│       └── USERNAME/
│           └── vault.remote/
├── seeds/
│   └── dendron.xkcd/
│       └── vault
├── dendron.yml
├── dendron.code-workspace
├── obsidian.templates/
│   └── daily.journal.md
├── obsidian.*/
├── .obsidian/
├── settings.code-workspace
├── .gitignore
└── README.md
```

### VSCode and Git

- `settings.code-workspace` the workspace for configurations and source control
- `.git*` Git dotfiles

### Dendron

- `notes` Dendron hierarchies notes
- `dendron.yml` Dendron config file
- `dendron.code-workspace` Dendron workspace
- `dependencies` multi vaults directory  
  Remote vaults: dedicated Git repositories
- `seeds` vaults shared by others, read-only

### Obsidian

- `.obsidian` Obsidian configurations
- `obsidian.*` notes that rely on Obsidian, e.g. `DataView`, `DB Folder` and `Longform`
