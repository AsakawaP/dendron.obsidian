# dendron.obsidian

> There is no loftier ambition than the pursuit of knowledge.

This project aims to explore a workflow to integrate the strengths of [Dendron][] and [Obsidian][] both :-)

[Dendron]: https://www.dendron.so
[Obsidian]: https://obsidian.md

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
├── obsidian.plugins/
├── .obsidian/
├── settings.code-workspace
├── .gitignore
└── README.md
```

### Dendron

- `notes` Dendron hierarchies notes
- `dendron.yml` Dendron config file
- `dendron.code-workspace` Dendron workspace
- `dependencies` multi vaults of the user  
  remote vaults are dedicated Git repositories
- `seeds` read-only vaults by others

### Obsidian

- `.obsidian` Obsidian configurations
- `obsidian.*` notes that rely on Obsidian, e.g. `DataView`, `DB Folder` and `Longform`

### VSCode and Git

- `settings.code-workspace` workspace to manage files in this repository  
  Markdown notes and cache files are excluded
- `.git*` Git dotfiles
