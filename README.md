# 夜话晓言 · 曾晓鹏文集

个人散文 / 随笔主页，陆续收存我写下的文字。品牌 / IP：夜话晓言（入夜成话，及晓成言）。

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
   `<a class="backlink" href="index.html">← 夜话晓言</a>`，
   再把 `dengshuikai.html` 顶部那段 `.backlink` 样式复制进该文件的 `<style>`。
3. 打开 `index.html`，在 `<ol class="entries">` 里复制一段 `<li class="entry">…</li>`，
   改成新文章的编号、标题、摘要、年份和链接。
4. 提交并推送：`git add . && git commit -m "新增：XXX" && git push`
   约一分钟后线上更新。

## 日间 / 夜间

主页与文章页右上角有 ☾/☀ 切换，选择会被浏览器记住（localStorage 键 `ye-theme`），首次访问跟随系统深色偏好，加载无闪烁。新文章想要同样效果，照搬 `dengshuikai.html` 的主题脚本（`<head>` 一段 + `</body>` 前一段）与 `.theme-toggle` 按钮、`[data-theme="dark"]` 样式即可，或直接交给我。

## 关于

纯静态 HTML，无需构建；本仓库独立管理。
（以后想绑定自定义域名、改版式或调整结构，告诉我即可。）
