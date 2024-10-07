# dendron.obsidian

> There is no loftier ambition than the pursuit of knowledge.

This repository tries to introduce a workflow to take advantages of [Dendron][] and [Obsidian][] both :-)

[Dendron]: https://www.dendron.so
[Obsidian]: https://obsidian.md

## Features

- Plaintext  
  Managing with Git
- Hierarchies notes  
  Designed by Dendron
- Cross-platform  
  Using Obsidian app

## File Structure

```plain-text
dendron.obsidian/
├── notes/
│   ├── .vscode/
│   │   └── dendron.code-snippets
│   ├── assets/
│   ├── root.md
│   ├── root.schema.yml
│   ├── dendron.hierarchy.md
│   └── obsidian.plugin.md
├── obsidian/
│   ├── templates/
│   │   └── daily.journal.md
│   ├── notes.dataview/
│   └── notes.dbfolder/
├── dependencies/
│   ├── localhost/
│   │   └── private.vault/
│   └── github.com/
│       └── AsakawaP/
│           └── public.vault/
├── seeds/
│   └── dendron.xkcd/
│       └── vault
├── .gitignore
├── .gitattributes
├── dendron.code-workspace
├── dendron.yml
├── settings.code-workspace
└── README.md
```
