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
<h3><ins>Preprints</ins></h3>
{% assign publications = site.preprints | sort: "number" | reverse %}
{% assign thesize = publications.size %}
{% for pub in publications %}
  <div class="pubitem">
    <div class="pubtitle"><td>[{{ thesize | minus: forloop.index | plus: 1 }}] </td><a href="{{pub.doi}}">{{ pub.title }}</a> </div>
    <div class="pubauthors">{{ pub.authors }}</div>
    <div class="pubinfo">{{ pub.publication }}, {{ pub.year}}</div>
    <div class="pubdoi"></div>
  </div>



<h3><ins>Peer-reviewed articles</ins></h3>

{% assign publications = site.publications | sort: "number" | reverse %}
{% assign thesize = publications.size %}
{% for pub in publications %}
  <div class="pubitem">
    <div class="pubtitle"><td>[{{ thesize | minus: forloop.index | plus: 1 }}] </td><a href="{{pub.doi}}">{{ pub.title }}</a> </div>
    <div class="pubauthors">{{ pub.authors }}</div>
    <div class="pubinfo">{{ pub.publication }}, {{ pub.year}}</div>
    <div class="pubdoi"></div>
  </div>
  
  
{% endfor %}


<h3><ins>PHD thesis</ins></h3>
<a href="/Downloads/WRAP_Theses_Monti_2020.pdf">Ultrafast Spectroscopy of Metal Halide Perovskites and III-V semiconductors</a>
, Maurizio Monti (2020)