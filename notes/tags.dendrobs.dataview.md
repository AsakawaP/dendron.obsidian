---
id: r5winop2exv8b2rwuoq3xb8
title: Dataview
desc: ''
updated: 1748132572961
created: 1745456216891
tags:
  - dendrobs.dataview
---

## Description

dv-desc:: Dataview => Dendron flavored multiple-hierarchy frontmatter tag

This tag `#dendrobs.dataview` lists some notes that contain commonly used  [[dendrobs.obsidian.plugin.dataview.publisher]] queries below.

Create your template notes with these [[dendrobs]] Dataview codeblock examples.

## Dendrobs Dataview Examples

%% DATAVIEW_PUBLISHER: start

```dataview
LIST WITHOUT ID "[[" + file.name + "]] " + dv-desc
FROM -"templates" AND -"seeds"
WHERE econtains(file.tags, regexreplace(this.file.name, "^tags\.", "#"))
SORT updated DESC
LIMIT 50
```

%%

- [[tags.dendrobs.dataview]] Dataview => Dendron flavored multiple-hierarchy frontmatter tag
- [[tags.dendrobs]] Dataview => Single-hierarchy tag (frontmatter or inline `#` hashtag), compatible with Obsidian
- [[dendrobs.obsidian]] Dataview => Dendron flavored index for all children of this note
- [[user.dendrobs.shakespeare]] Dataview => Markdown table output, compatible with Dendron
- [[user.kevinslin]] Dataview => Dendron flavored `@` user notes

%% DATAVIEW_PUBLISHER: end %%

***

## Description zh

dv-desc-zh:: Dataview => Dendron 风格的多层级 Frontmatter 标签

此标签 `#dendrobs.dataview` 列出了 *Dendron.Obsidian* 项目中包含 *Dataview Publisher* 常用查询的笔记。

可以利用这些笔记中的 Dataview 查询代码块示例，并结合你自己的需求创建模板。
