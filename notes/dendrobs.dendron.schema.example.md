---
id: r3ffaecm59ve5iwhk9hzhf5
title: Example
desc: ''
updated: 1736076046796
created: 1736075056485
---

## Date Format

```yaml
version: 1
schemas:
  - id: date
    title: date-schema
    parent: root
    desc: Date Schema
    children:
      - pattern: '[0-2][0-9][0-9][0-9]'
        desc: Year
        children:
          - pattern: 'Q[1-4]'
            desc: Season
            children:
              - pattern: '*'
                desc: Name
                template: templates.note
          - pattern: '[0-1][0-9]'
            desc: Month
            children:
              - pattern: '[0-3][0-9]'
                desc: Day
                template: templates.day
```
