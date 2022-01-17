---
layout: default
title: Album Covers
---
# Album Covers
{% assign sorted = site.albums | sort_natural:"sort_value" %}
{% for album in sorted -%}
<a href="{{ album.url }}"><img src="/assets/images/{{ album.date | date: "%Y/%m" }}/{{ album.cover }}" alt="{{ album.title }}" width=240></a>
{% endfor %}
