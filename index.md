---
layout: home
list_title: Notes and Updates
date: 2022-01-16
---
**Welcome to jazzofjapan.com**, a site for sharing information about Japanese Jazz and related music from Japanese musicians. 

* [Articles]({% link articles.md %}): List of the album reviews published here
* [Album Covers]({% link albums.md %}): List of the articles arranged by album covers
* [Musicians]({% link musicians.md %}): An index of musicians and albums
* [Audio]({% link audio.md %}): Audio excerpts for albums mentioned
* [Notes]({% link notes.md %}): News, updates, & miscellaneous notes

## Featured

{% assign latest = site.albums | where: "featured", "true" | sort: "date_updated" | reverse %}
{% assign img_width_latest = 140 %}
<table>
  <tbody>
    <tr>
{% for album in latest limit:3 -%}
<td class="spotlight"><a href="{{ album.url }}"><img class="spotlight" width={{ img_width_latest }} height={{ img_width_latest }} src="{% link assets/images/{{ album.date | date: "%Y/%m" }}/{{ album.cover }}-{{ img_width_latest }}.jpeg %}" alt="{{ album.title }}">
<br>
{{ album.artist }}:<br><em>{{ album.title }}</em></a>
<br>
<span class="subtext">{{ album.date_updated | date: "%b %e, %Y" }}</span>
<br>
</td>
{% endfor %}

   </tr>
  </tbody>
</table>


![Sax]({% link /assets/images/sax-shadow-1024.jpeg %})



