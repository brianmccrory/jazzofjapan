---
layout: default
title: Album Covers
---
# Album Covers

{% assign sorted = site.albums | sort_natural:"artist" %}
 {% for album in sorted -%}
<a href="{{ album.url }}"><img src="{{ site.baseurl }}/assets/images/{{ album.cover }}" alt="{{ album.title }}" width=240></a>
  {% endfor %}
