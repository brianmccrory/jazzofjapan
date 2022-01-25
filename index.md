---
layout: home
list_title: Notes and Updates
date: Jan 16, 2022
image: /assets/images/J-shaded.png
---
**Welcome to jazzofjapan.com**, a site for sharing information about Japanese Jazz and related music from Japanese musicians. 

* [Articles]({% link articles.md %}): List of the album reviews published here
* [Album Covers]({% link albums.md %}): List of the articles arranged by album covers
* [Musicians]({% link musicians.md %}): An index of musicians and albums
* [Audio]({% link audio.md %}): Audio excerpts for albums mentioned
* [Notes]({% link notes.md %}): News, updates, & miscellaneous notes


## Featured Albums

{% assign latest = site.albums | where: "featured", "true" | sort: "date_updated" | reverse %}


<table>
  <tbody>
    <tr>
	{%- assign sorted = site.albums | sort_natural:"sort_value" -%}
{% for album in latest limit:3 -%}
	{%- assign image = album.image | replace_first: "-460.jpeg", "-180.jpeg" -%}
<td class="spotlight"><a href="{{ album.url }}"><img class="spotlight" width=135 height=135 src="{{ image }}" alt="{{ album.title | escape }}">
<br>
{{ album.artist }}:<br><em>{{ album.title }}</em></a>
<br>
<span class="subtext">{{ album.date_updated | date: "%b %d, %Y" }}</span>
<br>
</td>
{% endfor %}
   </tr>
  </tbody>
</table>


![Sax]({% link /assets/images/sax-shadow-1024.jpeg %})



