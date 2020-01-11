---
layout: default
work: true
main: true
title: Writing My Idea
description: 글쓰기 작업
project-header: true
header-img: "img/project_bg.jpg"
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.writing == true %}

     {% include post-list.html %}

{% endif %}
{% endfor %}
</div>
