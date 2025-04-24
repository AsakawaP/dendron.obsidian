---
id: r3ffaecm59ve5iwhk9hzhf5
title: Example
desc: ''
updated: 1745475831001
created: 1736075056485
---

## Date-Tracking Schema

This date-tracking schema is extracted from Dendron default [Daily Journal Schema](./dendron.daily.schema.yml).[^1]

- `id: foo` this schema will match all notes whose filename starts with the prefix `foo.`
- `template: templates.day` this template will be applied automatically when creating a note with the name `foo.YEAR.MONTH.DAY`, e.g. `foo.2024.12.25`
- `template: templates.some-template-note` similar to the daily note, this template will be applied to `foo.YEAR.MONTH.DAY.*`, the asterisk symbol `*` is a wildcard.  

```yaml
version: 1
schemas:
  - id: foo
    title: date-tracking-schema
    parent: root
    desc: Date Tracking Schema
    children:
      - pattern: '[0-2][0-9][0-9][0-9]'
        desc: Year
        children:
          - pattern: '[0-1][0-9]'
            desc: Month
            children:
              - pattern: '[0-3][0-9]'
                desc: Day
                template: templates.day
                children:
                  - pattern: '*'
                    desc: Any Name
                    template: templates.some-template-note
          - pattern: 'Q[1-4]'
            desc: Season
```

Example:

Replace `id: foo` to `id: movie`, and `template: templates.some-template-note` to `template: templates.movie`.
Then you can create a movie-watching record like `movie.2024.12.25.千と千尋の神隠し`.

***

## 日期型笔记模式

日期型笔记模式来自 Dendron 默认的 [Daily Journal Schema](./dendron.daily.schema.yml)。[^2]

- `id: foo` 此模式将匹配所有文件名起始为 `foo.` 的笔记
- `template: templates.day` 此模板将在创建形如 `foo.年.月.日` 的笔记时自动应用
- `template: templates.some-template-note` 与每日笔记相仿，此模板将在形如 `foo.年.月.日.*` 的笔记创建时自动应用，星号符号 `*` 为通配符

```yaml
version: 1
schemas:
  - id: foo
      # 'id' 是文件名中点号分隔的字符串，按需修改
      # 此处表示匹配文件名起始为 foo. 的笔记
    parent: root
    title: 笔记标题 搜索时显示在右侧
      # 如 title 为空，显示匹配模式 'pattern'
    desc: 对 schema 的描述 在执行 'Lookup (Schema)' 时显示在 schema 文件名下方
    children:
      - pattern: '[0-2][0-9][0-9][0-9]'
        desc: 年度 形如 '2024'
        children:
          - pattern: '[0-1][0-9]'
            desc: 月度 形如 '12'
            children:
              - pattern: '[0-3][0-9]'
                desc: 日期 形如 '25'
                template: templates.day
                  # 日期笔记模板的文件名
                children:
                  - pattern: '*'
                    desc: 匹配笔记名 任意文本
                    template: templates.some-template-note
                      # 模版笔记的文件名
          - pattern: 'Q[1-4]'
            desc: 季度 形如 'Q4'
```

使用示例：

将起始域 `id: foo` 修改为 `movie`，并将 `template: templates.some-template-note` 修改为 `template: templates.movie`。
你就可以创建形如 `movie.2024.12.25.千与千寻` 的观影记录，并自动应用 `templates.movie` 模板。

***

[^1]: If `dendron.daily.schema.yml` does not exist, run the command `Dendron: Create Daily Journal Note` to release Dendron default schema file and create a, mostly the first, daily note.  

[^2]: 如果 `dendron.daily.schema.yml` 不存在，运行命令 `Dendron: Create Daily Journal Note` 会将 Dendron 的默认模式文件释放到仓库中，并创建一个（通常也是第一个）每日笔记。
