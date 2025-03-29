---
id: sy1v39gudb52b36lgu88wdi
title: Dendrobs
desc: ''
updated: 1743230860148
created: 1734608184229
---

## MOC of dendron.obsidian

%% DATAVIEW_PUBLISHER: start

```dataview
LIST WITHOUT ID regexreplace(file.name, "(.+)", "[[$1]]")
WHERE
  startswith(file.name, "dendrobs.")
  AND contains(file.tags, regexreplace(this.file.name, "^tags\.", ""))
SORT updated DESC
LIMIT 10
```

%%

- [[dendrobs.obsidian.plugin.structured-tree]]

%% DATAVIEW_PUBLISHER: end %%
