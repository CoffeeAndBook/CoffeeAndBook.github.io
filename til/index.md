---
layout: default
work: true
main: true
title: TIL
description: Today I Learned
project-header: true
header-img: "img/project_bg.jpeg"
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.til == true %}

     {% include post-list.html %}

{% endif %}
{% endfor %}

</div>
