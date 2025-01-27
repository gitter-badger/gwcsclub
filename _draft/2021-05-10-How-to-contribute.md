---
layout: page
title: 网站贡献指南
Author: ["Mark Chen"]
---

> Deprecated Page.

首先，如果你打开这个页面，说明你想成为网站的贡献者之一。 我们十分欢迎你的加入！

这个页面会详细的描述如何将自己的文章加入网站并正确的配置自己的文章内容使文章内容达到最好的展示效果。

### 0 - 文章写作

在完成一个页面前，我们需要先将自己准备展示的内容使用 Markdown 语言进行书写，并按照这个格式进行命名 - `yyyy-mm-dd-title-of-document.md`。 这里的 `yyyy-mm-dd` 是文章的创建日期。 这里的日期会被用于首页的“最新文章”栏目的自动生成与网页链接生成，所以请按照正确的格式填写。 文章的文件名中不能有空格，空格可以使用`-` 来代替。

> 例子：
>
> 如果我有一个文件是 2020 年 4 月 24 日 创建的，并且我想让他的标题是 `title of document`，那么我最后的 Markdown 文件应该是这个标题 - `2020-04-24-title-of-document.md`

<div class="info">
	<p>关于 Markdown 的格式与语法，请参考这个页面 - <a href="https://markdown.com.cn/basic-syntax/">Markdown 基本语法</a></p>
</div>

### 1 - 内容规范

完成内容的 Markdown 后，为了最好的展示效果，我们要保证 Markdown 文件的内容符合以下的内容规范

1. 【强制】 不使用一级标题，最高级的标题需要从二级标题开始
2. 【强制】 使用加粗 / 斜体等 Markdown 语法时，使用 \* 格式而不是 `_` 的下划线格式
3. 【强制】 如果使用 `==` 的语法表示高亮文字，需要将内容替换为 `&lt;mark&gt;` 标签。
4. 【强制】 如果在文件中添加了图片，需要将图片上传到第三方图床 / 在线对象存储等服务，否则会导致文件图片无法加载。
5. 【强制】 所有与网站内资源的路径使用 `{% raw %}{{ site.baseurl }}{% endraw%}` + 相对路径 替换绝对路径。 例如 `gwcompsci.gitee.io/assets/1.png` 应该转化为 {% raw %}`{{site.baseurl}}/assets/1.png`{% endraw %}
6. 【建议】 文件内最好只使用 2 到 4 级标题
7. 【建议】 上传前确认内容无误，样式正常

完成以上七条规范的修改后，需要在文件顶部加入 YAML 文件头，具体格式如下

```markdown
---
layout: 
title: 
author: 
tags: 
---
```

### 2 - 内容上传


