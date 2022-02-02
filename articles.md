---
title: Articles
image: /assets/images/J-shaded.jpg
---

# Articles 

{% assign sorted = site.albums | sort_natural: "sort_value" %}
{% for album in sorted -%}
1. [{{ album.artist }}: *{{ album.title }}*]({{ album.url }})
{% endfor %}

---

*Looking for specific musicians, albums, or other terms? [Search this site]({% link search.md %})*
