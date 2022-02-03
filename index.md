---
layout: home
list_title: Notes and Updates
image: /assets/images/J-shaded.jpg
---
**Welcome to jazzofjapan.com**, a site for sharing information about Japanese Jazz and related music from Japanese musicians. 

* [Articles]({% link articles.md %}): List of the album reviews published here
* [Album Covers]({% link albums.md %}): List of the articles arranged by album covers
* [Musicians]({% link musicians.md %}): An index of musicians and albums
* [Audio]({% link audio.md %}): Audio excerpts for albums mentioned
* [Notes]({% link notes.md %}): News, updates, & miscellaneous notes

## Featured Albums

{%- assign new = site.albums | where: "featured", "true" | where: "date_updated", nil | sort: "date" | reverse | limit: 3 -%}
{%- assign updated_size = 3 | minus: new.size -%}
{%- if updated_size > 0 -%}
{%- assign updated = site.albums | where: "featured", "true" | sort: "date_updated" | reverse | limit: updated_size -%}
{%- endif %}
<table>
  <tbody>
    <tr>
{% for album in new limit:3 -%}
{% include featured.md %}
{% endfor %}
{% for album in updated limit: updated_size -%}
{% include featured.md %}
{% endfor %}
   </tr>
  </tbody>
</table>


## Latest Articles
{%- assign latest_new = site.albums | sort: "date" | reverse -%}
{%- assign latest_updated = site.albums | sort: "date_updated" | reverse %}
<table><tbody><tr><td class="latest">
<em>New:</em><br>
<ul>
{% for album in latest_new limit:3 -%}
<li><a href="{{ album.url }}">{{ album.artist | escape }}: <em>{{ album.title | escape }}</em></a> <span class="subtext">{{ album.date | date: "%b %e, %Y" }}</span></li>
{% endfor %}
</ul>
</td><td class="latest">
<em>Updated:</em><br>
<ul>
{% for album in latest_updated limit: 3 -%}
<li><a href="{{ album.url }}">{{ album.artist | escape }}: <em>{{ album.title | escape }}</em></a> <span class="subtext">{{ album.date_updated | date: "%b %e, %Y" }}</span></li>
{% endfor %}
</ul>
</td></tr></tbody></table>


![Sax]({% link /assets/images/sax-shadow-1024.jpeg %})



