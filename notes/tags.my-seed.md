---
id: sy1v39gudb52b36lgu88wdi
title: My Seed
desc: ''
updated: 1750240600017
created: 1734608184229
tags:
  - my-seed.dataview
---

## MOC of dendron.obsidian

%% DATAVIEW_PUBLISHER: start

```dataview
LIST WITHOUT ID "[[" + file.name + "]]"
FROM -"templates" AND -"seeds"
WHERE
  econtains(file.tags, regexreplace(this.file.name, "^tags\.", "#"))
  AND startswith(file.name, "my-seed.")
SORT file.name ASC
LIMIT 50
```

%%

- [[my-seed.obsidian.plugin.structured-tree]]

%% DATAVIEW_PUBLISHER: end %%

***

## Description

dv-desc:: Dataview => Single-hierarchy tag (frontmatter or inline `#` hashtag), compatible with Obsidian

dv-desc-zh:: Dataview => 兼容 Obsidian 的单层级标签，支持 Frontmatter 或正文中 `#` 标签
