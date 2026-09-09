---
title: "News"
layout: textlay
excerpt: "VMD Lab at University of Tokyo."
sitemap: false
permalink: /allnews.html
---

# News

{% assign sorted_news = site.data.news | sort: "sortdate" | reverse %}
{% for article in sorted_news %}
<b>{{ article.date }}</b> <br>
{{ article.headline | markdownify}} <br>
{% endfor %} 
