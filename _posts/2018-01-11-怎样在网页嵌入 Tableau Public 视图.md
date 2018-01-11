---
layout: article
title:  "如何在 iFrame 中嵌入 Tableau Public 视图"
date:   2017-01-11 21:14:24 +0800
categories: infovis
image:
  teaser: iframe.jpg
  feature: iframe.jpg
---
## 如何在 iFrame 中嵌入 Tableau Public 视图
1. 转到 Tableau Public 中的视图。
2. 选择视图底部的“共享”选项，并复制“链接”部分中提供的链接。
3. 在 iframe 代码中添加该链接。
4. 在 iFrame 中嵌入 Tableau Public 视图时，URL 必须包括以下参数：

```
showVizHome=no 
embed=true 
```


可参考以下例子：
```
<iframe src="https://public.tableau.com/views/GDPPOP/1_1?:embed=y&:display_count=yes&publish=yes/Dashboard1?:showVizHome=no&:embed=true"
				width="645" height="955"></iframe>"
```

5. 注意：将视图的 URL 用于 iframe src 属性时，不要包括 URL 最末尾的数字符号 (#) 和数字。
- 正确的 src 内容：

```
https://public.tableausoftware.com/views/public_exercise/Dashboard1?:showVizHome=no&:embed=true
```
- 不正确的 src 内容：

```
https://public.tableausoftware.com/views/public_exercise/Dashboard1?:showVizHome=no&:embed=true#2
```
6. 为确保默认情况下在嵌入视图中显示原始视图，请确保名称参数的嵌入代码 URL 未显式引用自定义视图，并在嵌入代码中包含以下筛选器参数：

```
<param name="filter" value=":original_view=yes"/>。
```


以上是关于怎样利用iframe在网页嵌入 Tableau Public 视图的一些笔记，具体内容参考Tableau Public 官方知识库