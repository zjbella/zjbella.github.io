---
layout: page
title: 关于
keywords: zjbella
comments: false
menu: 关于
permalink: /about/
---

## 联系

<ul>
{% for website in site.data.social %}
<li>{{ website.sitename }}：<a href="{{ website.url }}" target="_blank" rel="noopener">@{{ website.name }}</a></li>
{% endfor %}
</ul>

## 技能关键词

{% for skill in site.data.skills %}
### {{ skill.name }}
<p class="chips">{% for keyword in skill.keywords %}<span class="tag">{{ keyword }}</span>{% endfor %}</p>
{% endfor %}