---
title: Notes
image: /assets/images/J-shaded.jpg
---
# News, Updates, & Miscellaneous Notes

{% assign posts = site.posts %}

<ul class="post-list">
{%- for post in posts -%}
<li>
<span class="post-meta">{{ post.date | date: "%b %e, %Y" }}</span>
<h3><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h3>
</li>
{%- endfor -%}
</ul>
