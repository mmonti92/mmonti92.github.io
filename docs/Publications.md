---
layout: page
title: "Publications"
permalink: /Publications/
order: 5
---

<style type="text/css">
 .pubitem {
  margin: 2em 0;
  line-height: 1em;
}

.pubtitle {
  margin-bottom: 0.5em;
  line-height: 1.2em;
  font-weight: bold;
}

.pubauthors,
.pubinfo {
  font-size: 75%;
  margin-bottom: 0.75em;
}



</style>
{% assign publications = site.publications | sort: "number" | reverse %}
{% assign thesize = publications.size %}
{% for pub in publications %}
  <div class="pubitem">
    <div class="pubtitle"><td>[{{ thesize | minus: forloop.index | plus: 1 }}] </td>{{ pub.title }} </div>
    <div class="pubauthors">{{ pub.authors }}</div>
    <div class="pubinfo">{{ pub.publication }}, {{ pub.year}}</div>
  </div>
{% endfor %}
