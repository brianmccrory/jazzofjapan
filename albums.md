---
layout: default
title: Album Covers
image: /assets/images/J-shaded.jpg
---
# Album Covers
{% assign img_width = "240" %}
{% assign img_resize = "-" | append: img_width | append: ".jpeg" %}
{% assign sorted = site.albums | sort_natural:"sort_value" %}
{% for album in sorted -%}
{%- assign image = album.image | replace_first: "-460.jpeg", img_resize -%}
<a href="{{ album.url }}"><img class="albumgrid" src="{{ image }}" alt="{{ album.title | escape }}" width={{ img_width }} height={{ img_width }}></a>
{% endfor %}
