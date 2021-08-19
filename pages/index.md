---
layout: page
title: SRCC Documentation Portal
permalink: /
---

# Welcome to Hoon Lab

### Our lab is Computational Biomedicine [@hoonbiolab](https://twitter.com/hoonbiolab).

<style>
@import url(https://fonts.googleapis.com/css?family=Roboto:400,300,300italic,100,100italic,400italic,500,500italic,700,700italic&subset=latin,cyrillic);

<h2>Rescent News</h2>
<div class="wrapper">
  {% for service in site.data.metadata.services %}<div class="box">
  <div class="text">
    <div class="title">{{ service.name }}</div>
      <p><img src="{{ service.logo }}" style="height:140px; position:absolute">
       <span style="width:50%; float:right">{{ service.description }}</span>
      </p>
    </div>
    <div class="act">
	<a href="{{ service.url }}" target="_blank"><div class="card-button">Documentation</div></a>
    </div>
  </div>{% endfor %}
</div>

<h2>Resources</h2>
<div class="wrapper">
  {% for resource in site.data.metadata.resources %}<div class="box">
  <div class="text">
    <div class="title">{{ resource.name }}</div>
      <p><img src="{{ resource.logo }}" style="height:160px; position:absolute">
       <span style="width:50%; float:right">{{ resource.description }}</span>
      </p>
    </div>
    <div class="act">
	<a href="{{ resource.url }}" target="_blank"><div class="card-button">Documentation</div></a>
    </div>
  </div>{% endfor %}
</div>

For getting started with a general linux cluster, see the {% include doc.html name="Getting Started" path="getting-started" %} page. If you need help or want to improve the site, please [open an issue]({{ site.repo }}/issues) or
contact us at [{{ site.email }}](mailto:{{ site.email }})
