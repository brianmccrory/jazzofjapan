{%- assign image = album.image | replace_first: "-460.jpeg", "-140.jpeg" -%}
<td class="spotlight"><a href="{{ album.url }}"><img class="spotlight" width=140 height=140 src="{{ image }}" alt="{{ album.title | escape }}"><br>
{{ album.artist | escape }}:<br><em>{{ album.title |escape }}</em></a><br>
{% if album.date_updated %}{% assign date_to_show = album.date_updated %}{% else %}{% assign date_to_show = album.date %}{% endif %}
<span class="subtext">{{ date_to_show | date: "%b %e, %Y" }}</span>
</td>