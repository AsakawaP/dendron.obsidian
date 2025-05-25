---
id: 82m1bzb94yvoqwtxhykkrth
title: William Shakespeare 威廉·莎士比亚
desc: ''
updated: 1748132616969
created: 1736742458279
tags:
  - dendrobs.dataview
---

%% DATAVIEW_PUBLISHER: start

```dataview
TABLE WITHOUT ID
"[[" + file.name + "]]" AS "File",
regexreplace(string(author), "\[\[[^|]+\|([^\]]+)\]\]", "[[$1]]") AS "Author",
title AS "Title"
FROM -"templates" AND -"seeds"
WHERE startswith(file.name, "dendrobs")
  AND econtains(author, this.file.link)
SORT file.name ASC
LIMIT 50
```

%%

| File                         | Author                        | Title         |
| ---------------------------- | ----------------------------- | ------------- |
| [[dendrobs.example.hamlet]]  | [[user.dendrobs.shakespeare]] | Hamlet 哈姆雷特   |
| [[dendrobs.example.lear]]    | [[user.dendrobs.shakespeare]] | King Lear 李尔王 |
| [[dendrobs.example.macbeth]] | [[user.dendrobs.shakespeare]] | Macbeth 麦克白   |
| [[dendrobs.example.othello]] | [[user.dendrobs.shakespeare]] | Othello 奥赛罗   |

%% DATAVIEW_PUBLISHER: end %%

***

## Description

dv-desc:: Dataview => Markdown table output, compatible with Dendron

dv-desc-zh:: Dataview => 输出兼容 Dendron 的 Markdown 表格
