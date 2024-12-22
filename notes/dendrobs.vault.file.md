---
id: dnqbcn8qnm69kpxo7ehew2t
title: File Structure
desc: ''
updated: 1734886698513
created: 1734575775311
---

## File Structure

```text
dendron.obsidian/
├── dendron.code-workspace
├── dendron.yml
├── notes/
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
├── templates/
│   └── daily.journal.md
├── obsidian.*/
├── settings.code-workspace
├── .gitignore
├── .gitattributes
└── README.md
```

## Dendron

- `dendron.code-workspace` Dendron workspace
- `dendron.yml` Dendron config file
- `notes` default note directory
- `dependencies` directory to integrate multi vaults
  - Local vault
    `dependencies/localhost/VAULT_NAME`  
    Self-contained vaults which managed by the main repository  
  - Remote vault
    `dependencies/github.com/USERNAME/REPOSITORY_NAME`  
    Self-contained vaults with source remote repositories on GitHub
    **Tip**: Keep directories the same as remote sources.  
- `seeds` vaults shared by others, treated as read-only
  **Tip**: In Dendron's early version (and official seeds), default note directories are `vault`.

## Obsidian

- `.obsidian` Obsidian configurations, themes and plugins
- `templates` template notes for Obsidian
- `obsidian.*` folders of notes which rely on Obsidian or are not suitable with Dendron  
  e.g. `Canvas`, `Longform`, `DB Folder`

## VSCode and Git

- `settings.code-workspace` the workspace for configurations and source control management
- `.gitignore` && `.gitattributes` Git config files
