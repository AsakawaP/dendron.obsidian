---
id: kovwq3qbdllhwtq3dcdjqnw
title: 硬核笔记 Dendron
desc: ''
updated: 1743091974207
created: 1743077431526
---

> [!NOTE]  
> 本文节选自博客 [智商帝 | 个人 PKM 折腾记](https://blog.l0v0.com/posts/afa065b7.html#Dendron)。  
> @my-seed.asakawap 在这篇文章中发现了 Dendron。

Dendron 是在 VScode 实现双链笔记的插件……
提供了 npm 命令行工具可以将自己的笔记生成对应的网站，并且支持文章引用嵌入。
  
Dendron 的作者推荐用扁平的目录结构来管理笔记，有点过于硬核。
作者推荐不使用文件夹，而是在文件上用 `.` 进行区分，当作文件夹使用，这样文件夹也有文件信息进行描述。

```text
dendron/
├── cli.tar.md
├── cli.tar.env.md
├── cli.curl.md
└── cli.dig.md

folder/
└── cli/
    |── dig.md
    |── curl.md
    |── tar.md
    └── tar/
        └── env.md
```

这样做的好处是可以通过搜索，快速找到命名相近的功能，利用 `cli.*.env` 之类的的通配符匹配。

偏平结构也方便程序检索，查找笔记的时候也不用一层层点击去找（特别是目录结构很深的情况）。
