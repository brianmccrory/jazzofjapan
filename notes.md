---
title: Notes
image: /assets/images/J-shaded.jpg
---
# News, Updates, & Miscellaneous Notes

{% assign posts = site.posts %}

<table><tr><td>
<h3>Latest Updates:</h3>
<ul>
{%- for post in posts -%}
{% if post.tag == "update" %}
<li><a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a> <span class="post-meta">({{ post.date | date: "%b %e, %Y" }})</span></li>
{% endif %}
{%- endfor -%}
</ul>
</td></tr></table>


<ul class="post-list">
{%- for post in posts -%}
{% if post.tag != "update" %}
<li>
<span class="post-meta">{{ post.date | date: "%b %e, %Y" }}</span>
<h3><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h3>
</li>
{% endif %}
{%- endfor -%}
</ul>