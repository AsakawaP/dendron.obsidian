---
id: sy1v39gudb52b36lgu88wdi
title: Dendrobs
desc: ''
updated: 1743073734715
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
```

%%

- [[dendrobs.obsidian.plugin.structured-tree]]

%% DATAVIEW_PUBLISHER: end %%
