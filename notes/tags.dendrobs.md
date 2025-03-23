---
id: sy1v39gudb52b36lgu88wdi
title: Dendrobs
desc: ''
updated: 1742719620244
created: 1734608184229
---

%%

```dataview
LIST
WHERE
  startswith(file.name, "dendrobs")
  AND icontains(file.tags, regexreplace(this.file.name, "tags\.", ""))
SORT updated DESC
LIMIT 10
```

%%

<details>
<summary>MOC of <b>dendron.obsidian</b></summary>

<!-- QueryToSerialize: LIST WHERE startswith(file.name, "dendrobs") AND icontains(file.tags, regexreplace(this.file.name, "tags\.", "")) SORT updated DESC -->
<!-- SerializedQuery: LIST WHERE startswith(file.name, "dendrobs") AND icontains(file.tags, regexreplace(this.file.name, "tags\.", "")) SORT updated DESC -->
- [[dendrobs.obsidian.plugin.structured-tree]]
<!-- SerializedQuery END -->

</details>
