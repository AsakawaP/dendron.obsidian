---
id: r5winop2exv8b2rwuoq3xb8
title: Dataview
desc: ''
updated: 1750240551502
created: 1745456216891
tags:
  - my-seed.dataview
---

## Description

dv-desc:: Dataview => Dendron flavored multiple-hierarchy frontmatter tag

#my-seed.dataview  
This tag lists some notes that contain commonly used [[my-seed.obsidian.plugin.dataview.publisher]] queries below.

Create your template notes with these [[my-seed]] Dataview codeblock examples.

## Dendron-Obsidian Dataview Examples

%% DATAVIEW_PUBLISHER: start

```dataview
LIST WITHOUT ID "[[" + file.name + "]] " + dv-desc
FROM -"templates" AND -"seeds"
WHERE econtains(file.tags, regexreplace(this.file.name, "^tags\.", "#"))
SORT file.name ASC
LIMIT 50
```

%%

- [[my-seed.example.shakespeare]] Dataview => Markdown table output, compatible with Dendron
- [[my-seed.obsidian]] Dataview => Dendron flavored index for all children of this note
- [[tags.my-seed]] Dataview => Single-hierarchy tag (frontmatter or inline `#` hashtag), compatible with Obsidian
- [[tags.my-seed.dataview]] Dataview => Dendron flavored multiple-hierarchy frontmatter tag
- [[user.kevinslin]] Dataview => Dendron flavored `@` user notes

%% DATAVIEW_PUBLISHER: end %%

***

## Description zh

dv-desc-zh:: Dataview => Dendron 风格的多层级 Frontmatter 标签

#my-seed.dataview  
此标签列出了 *Dendron.Obsidian* 项目中包含 *Dataview Publisher* 常用查询的笔记。

可以利用这些笔记中的 Dataview 查询代码块示例，并结合你自己的需求创建模板。

## Dendron-Obsidian Dataview Examples zh

%% DATAVIEW_PUBLISHER: start

```dataview
LIST WITHOUT ID "[[" + file.name + "]] " + dv-desc-zh
FROM -"templates" AND -"seeds"
WHERE econtains(file.tags, regexreplace(this.file.name, "^tags\.", "#"))
SORT file.name ASC
LIMIT 50
```

%%

- [[my-seed.example.shakespeare]] Dataview => 输出兼容 Dendron 的 Markdown 表格
- [[my-seed.obsidian]] Dataview => Dendron 风格的目录，列出此笔记的所有子项
- [[tags.my-seed]] Dataview => 兼容 Obsidian 的单层级标签，支持 Frontmatter 或正文中 `#` 标签
- [[tags.my-seed.dataview]] Dataview => Dendron 风格的多层级 Frontmatter 标签
- [[user.kevinslin]] Dataview => Dendron 风格 `@` 用户笔记

%% DATAVIEW_PUBLISHER: end %%
