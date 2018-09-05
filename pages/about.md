---
layout: page
title: About
description: 代码改变世界
keywords: Connor
comments: true
menu: 关于
permalink: /about/
---

Make English as your working language.
Practice makes perfect.
All experience comes from mistakes.
Don't be one of the leeches.
Either stand out or kicked out.

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
