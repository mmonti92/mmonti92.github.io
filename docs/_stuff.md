---
layout: page
title: Research
nav: true
siteNav: true
---
<a href="{{ staff_member.url }}">
      {{ staff_member.name }}
{% for r in site.research_item %}
 <h2><a href="{{ r.url }}">{{ r.title }}</a></h2>
{% endfor %}