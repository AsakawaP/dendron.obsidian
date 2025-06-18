---
id: 82m1bzb94yvoqwtxhykkrth
title: William Shakespeare 威廉·莎士比亚
desc: ''
updated: 1750238852412
created: 1736742458279
tags:
  - my-seed.dataview
---

## Dataview Query

%% DATAVIEW_PUBLISHER: start

```dataview
TABLE WITHOUT ID
  "[[" + file.name + "]]" AS "File",
  regexreplace(string(author), "\[\[[^|]+\|([^\]]+)\]\]", "[[$1]]") AS "Author",
  title AS "Title"
FROM -"templates" AND -"seeds"
WHERE econtains(author, this.file.link)
  AND startswith(file.name, "my-seed.")
SORT file.name ASC
LIMIT 50
```

%%

| File                        | Author                       | Title         |
| --------------------------- | ---------------------------- | ------------- |
| [[my-seed.example.hamlet]]  | [[my-seed.example.shakespeare]] | Hamlet 哈姆雷特   |
| [[my-seed.example.lear]]    | [[my-seed.example.shakespeare]] | King Lear 李尔王 |
| [[my-seed.example.macbeth]] | [[my-seed.example.shakespeare]] | Macbeth 麦克白   |
| [[my-seed.example.othello]] | [[my-seed.example.shakespeare]] | Othello 奥赛罗   |

%% DATAVIEW_PUBLISHER: end %%

***

## Description

dv-desc:: Dataview => Markdown table output, compatible with Dendron

dv-desc-zh:: Dataview => 输出兼容 Dendron 的 Markdown 表格
