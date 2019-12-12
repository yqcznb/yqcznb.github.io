---
layout: page
title: About
description: 我就是我
keywords: Yin Qichen, 尹琦琛
comments: true
menu: 关于
permalink: /about/
---

我是阿琛，追随时代步伐，敢于弄潮。

相信技术改变生活。

哪有什么胜利可言，挺住意味着一切！

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
