---
layout: default
title: Album Covers
---
{% assign image_width = "240" %}
# Album Covers
{% assign sorted = site.albums | sort_natural:"sort_value" %}
{% for album in sorted -%}
<a href="{{ album.url }}"><img class="albumgrid" src="/assets/images/{{ album.date | date: "%Y/%m" }}/{{ album.cover }}-{{ image_width }}.jpeg" alt="{{ album.title }}" width={{ image_width }} height={{ image_width }}></a>
{% endfor %}
