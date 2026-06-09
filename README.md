# 曾晓鹏 · 文集

个人散文 / 随笔主页，陆续收存我写下的文字。

- **线上地址**：https://zengxiaopeng-code.github.io/essays/

## 结构

```
.
├── index.html        # 主页：文章列表
├── dengshuikai.html  # 文章：等水开 — 债务临界、美元换锚……
└── README.md
```

每篇文章都是一个自带样式、可独立打开的 HTML 文件，直接放在仓库根目录。

## 怎么新增一篇文章

1. 把新文章的 HTML 放进仓库根目录，文件名用简短拼音/英文，例如 `xinpian.html`。
2. （推荐）给文章加返回链接：在 `<main class="wrap">` 之后加一行
   `<a class="backlink" href="index.html">← 文集 · 曾晓鹏</a>`，
   再把 `dengshuikai.html` 顶部那段 `.backlink` 样式复制进该文件的 `<style>`。
3. 打开 `index.html`，在 `<ol class="entries">` 里复制一段 `<li class="entry">…</li>`，
   改成新文章的编号、标题、摘要、年份和链接。
4. 提交并推送：`git add . && git commit -m "新增：XXX" && git push`
   约一分钟后线上更新。

## 关于

纯静态 HTML，无需构建；本仓库独立管理。
（以后想绑定自定义域名、改版式或调整结构，告诉我即可。）
