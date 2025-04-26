---
id: 9ub5ovtcemqwbjaz3pq08mz
title: Kevin Lin
desc: ''
updated: 1745579753395
created: 1735304738957
tags:
  - dendrobs.dataview
---

{{fm.title}} is the founder and CEO of [[dendrobs.dendron]].

- [Personal HomePage](https://www.kevinslin.com)
- [GitHub](https://github.com/kevinslin)

***

%% DATAVIEW_PUBLISHER: start

```dataview
LIST WITHOUT ID "[[" + file.name + "]]"
FROM -"templates" AND -"seeds"
WHERE
  dendrobs-user = "@" + regexreplace(this.file.name, "^user.", "")
SORT updated DESC
LIMIT 50
```

%%

- [[dendrobs.resource.its-your-knowledge-base]]
- [[dendrobs.resource.how-to-index-10000-notes]]

%% DATAVIEW_PUBLISHER: end %%

***

## Description

dv-desc:: Dataview => Dendron flavored `@` user notes

dv-desc-zh:: Dataview => Dendron 风格 `@` 用户笔记
