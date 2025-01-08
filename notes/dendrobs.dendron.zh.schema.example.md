---
id: 33mtuzpqwgvwew6lu46ekc8
title: Example
desc: ''
updated: 1736333324514
created: 1736330324471
---

## 日期季度类笔记结构

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
          - pattern: 'Q[1-4]'
            desc: 季度 形如 'Q4'
            children:
              - pattern: '*'
                desc: 匹配笔记名 任意文本
                template: templates.note
                # 模版笔记的文件名
```

使用示例：  
将起始域修改为 `book` 并创建 `templates.book` 并修改 `templates.day` 为对应模板  
就可以使用模板创建如 `book.2024.12.25.图书名` 的阅读记录
