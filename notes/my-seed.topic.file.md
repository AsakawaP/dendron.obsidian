---
id: dnqbcn8qnm69kpxo7ehew2t
title: File Structure
desc: ''
updated: 1750233827724
created: 1734575775311
---

## File Structure

```text
dendron.obsidian/
├── .vscode/
│   └── settings.json
├── dendron.code-workspace
├── dendron.yml
├── notes/
│   └── assets/
├── dependencies/
│   ├── localhost/
│   │   └── local_vault/
│   │       └── notes/
│   └── github.com/
│       └── USERNAME/
│           └── remote_vault/
│               └── notes/
├── seeds/
│   └── dendron.dendron-site/
│       └── vault/
├── .obsidian/
├── obs.*/
├── templates/
│   └── daily.journal.md
├── scripts/
├── .gitignore
├── .gitattributes
└── README.md
```

## Dendron

- `dendron.code-workspace` Dendron workspace
- `dendron.yml` Dendron config file
- `notes` default note directory
  - `assets` attachment files directory
- `dependencies` directory to integrate multi vaults
  - Local vault
    `dependencies/localhost/VAULT_NAME`  
    Self-contained vaults which managed by the main repository  
  - Remote vault
    `dependencies/github.com/USERNAME/REPOSITORY_NAME`  
    Self-contained vaults with source remote repositories on GitHub
    **Tip**: Keep directories the same as remote sources.  
- `seeds` vaults shared by others, treated as read-only
  **Tip**: In Dendron's early version (and official seeds), the default note directory name is `vault`.

## Obsidian

- `.obsidian` Obsidian configurations, themes and plugins
- `templates` template notes for Obsidian
- `obs.*` folders of notes which rely on Obsidian or are not suitable with Dendron  
  E.g. `Obsidian Canvas`, `Longform`

## VSCode and Git

- `settings.json` settings of the Root directory
- `.gitignore` && `.gitattributes` Git config files
- `scripts` user scripts
  E.g. [[my-seed.obsidian.plugin.templater]] user scripts
