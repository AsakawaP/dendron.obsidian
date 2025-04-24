---
id: sy1v39gudb52b36lgu88wdi
title: Dendrobs
desc: ''
updated: 1745466892832
created: 1734608184229
tags:
  - dendrobs.dataview
---

## MOC of dendron.obsidian

%% DATAVIEW_PUBLISHER: start

```dataview
LIST WITHOUT ID "[[" + file.name + "]]"
FROM -"templates" AND -"seeds"
WHERE
  startswith(file.name, "dendrobs.")
  AND contains(file.tags, regexreplace(this.file.name, "^tags\.", ""))
SORT updated DESC
LIMIT 10
```

%%

- [[dendrobs.obsidian]]
- [[dendrobs.obsidian.plugin.structured-tree]]

%% DATAVIEW_PUBLISHER: end %%

***

## Description

dv-desc:: Dataview => Single-hierarchy tag (frontmatter or inline `#` hashtag), compatible with Obsidian

dv-desc-zh:: Dataview => 兼容 Obsidian 的单层级标签，支持 Frontmatter 或正文中 `#` 标签
