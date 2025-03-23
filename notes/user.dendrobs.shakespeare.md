---
id: 82m1bzb94yvoqwtxhykkrth
title: William Shakespeare 威廉·莎士比亚
desc: ''
updated: 1742719541559
created: 1736742458279
---

## Dataview Query

%%

```dataview
LIST
WHERE startswith(file.name, "dendrobs")
  AND author = this.file.link
SORT file.name ASC
LIMIT 10
```

%%

## Serialized Query

<!-- QueryToSerialize: LIST WHERE startswith(file.name, "dendrobs") AND author = this.file.link SORT file.name ASC -->
<!-- SerializedQuery: LIST WHERE startswith(file.name, "dendrobs") AND author = this.file.link SORT file.name ASC -->
- [[dendrobs.example.hamlet]]
- [[dendrobs.example.lear]]
- [[dendrobs.example.macbeth]]
- [[dendrobs.example.othello]]
<!-- SerializedQuery END -->
