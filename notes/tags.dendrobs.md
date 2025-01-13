---
id: sy1v39gudb52b36lgu88wdi
title: Dendrobs
desc: ''
updated: 1734979618156
created: 1734608184229
---

%%

```dataview
LIST
FROM "" AND -"seeds"
WHERE icontains(file.tags, regexreplace(this.file.name, "tags\.", ""))
SORT updated DESC
```

%%

<details>
   <summary><b>MOC of dendron.obsidian</b></summary>

<!-- QueryToSerialize: LIST FROM "" AND -"seeds" WHERE icontains(file.tags, regexreplace(this.file.name, "tags\.", "")) SORT updated DESC -->
<!-- SerializedQuery: LIST FROM "" AND -"seeds" WHERE icontains(file.tags, regexreplace(this.file.name, "tags\.", "")) SORT updated DESC -->
- [[dendrobs.obsidian.plugin.structured-tree]]
<!-- SerializedQuery END -->

</details>
