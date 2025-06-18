---
id: 9ub5ovtcemqwbjaz3pq08mz
title: Kevin Lin
desc: ''
updated: 1750236361037
created: 1735304738957
tags:
  - my-seed.dataview
---

{{fm.title}} is the founder and CEO of [[my-seed.dendron]].

- [Personal HomePage](https://www.kevinslin.com)
- [GitHub](https://github.com/kevinslin)

***

%% DATAVIEW_PUBLISHER: start

```dataview
LIST WITHOUT ID "[[" + file.name + "]]"
FROM -"templates" AND -"seeds"
WHERE
  seed-example-user = "@" + regexreplace(this.file.name, "^user.", "")
SORT file.name ASC
LIMIT 50
```

%%

- [[my-seed.resource.its-your-knowledge-base]]
- [[my-seed.resource.how-to-index-10000-notes]]

%% DATAVIEW_PUBLISHER: end %%

***

## Description

dv-desc:: Dataview => Dendron flavored `@` user notes

dv-desc-zh:: Dataview => Dendron 风格 `@` 用户笔记
