---
id: 82m1bzb94yvoqwtxhykkrth
title: William Shakespeare 威廉·莎士比亚
desc: ''
updated: 1743075139076
created: 1736742458279
---

%% DATAVIEW_PUBLISHER: start

```dataview
LIST WITHOUT ID regexreplace(file.name, "(.+)", "[[$1]]")
FROM -"seeds"
WHERE startswith(file.name, "dendrobs")
  AND author = this.file.link
SORT file.name ASC
```

%%

- [[dendrobs.example.hamlet]]
- [[dendrobs.example.lear]]
- [[dendrobs.example.macbeth]]
- [[dendrobs.example.othello]]

%% DATAVIEW_PUBLISHER: end %%
