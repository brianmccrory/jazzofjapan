---
layout: default
title: Albums
---
<h1>Albums</h1>

 {% assign sorted = site.albums | sort: 'date' | reverse %}
 {% for album in sorted %}
<figure>
<a href="{{ album.url }}"><img src="{{ site.baseurl }}/assets/images/{{ album.cover }}" alt="{{ album.title }}"></a>
<figcaption><em><a href="{{ album.url }}">{{ album.title }}</a></em> by {{ album.artist }}</figcaption>
</figure>
  {% endfor %}
