---
layout: main
title:  "News"
date:   2022-02-16 20:18:25 +0000
categories: news
---

{% for news in site.news reversed %}
{{ news.date | date: "%d %b %Y" }}&nbsp;&nbsp;-&nbsp;&nbsp;[{{ news.title }}]({{ news.url }})
{% endfor %}
