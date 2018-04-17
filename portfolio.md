---
layout: cv
title: Javi Ballester Portfolio
permalink: portfolio/
extra_css: portfolio.css
---

Javi Ballester
==============

Curriculum Vitae

<div id="webaddress"><a class="screen" href="/">Printable CV</a></div>

## Image samples

{% assign years = "17, 15, 14, 13, 12, 09, 08, 07, 05, 04, 03, 02" | split: ", " %}{% for year in years %}{% capture cont %}/images/mostra/{{ year }}{% endcapture %}
### 20{{year}}
<div id="thumbs">
{% for image in site.static_files %}{% if image.path contains cont %}
<a href="{{ site.baseurl }}{{ image.path }}" target="_blank">
<span class="w3-hover-opacity" style="background-image:url('{{ site.baseurl }}/images/thumbs/thumb_{{ image.name | remove: image.extname }}.png');">
</span>
</a>
{% endif %}{% endfor %}
</div>
{% endfor %}

## Last update

April 2018


