---
layout: post
title: المقالات
description: مقالات قناة عالم الألعاب عن eFootball واللاعيبة المجانيين.
---
{% assign items = site.pages | where: "layout", "post" | reverse %}
<ul class="alist">
{% for p in items %}{% unless p.url == page.url %}
<li><a href="{{ p.url }}">{{ p.title }}</a></li>
{% endunless %}{% endfor %}
</ul>
