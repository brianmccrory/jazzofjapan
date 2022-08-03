---
layout: home
list_title: Notes and Updates
image: /assets/images/J-shaded.jpg
---
**This is jazzofjapan.com**, a site about Japanese jazz and related music from Japanese musicians. 

*New!* Exclusive content at [Buy me a coffee](https://www.buymeacoffee.com/brmc)!

_Latest Articles_
{%- assign latest_type = "new" -%}
{%- assign latest_new = site.albums | sort: "date" | reverse %}
<table>
  <tbody>
    <tr>
{% for album in latest_new limit:3 -%}
{% include featured.md %}
{% endfor %}
   </tr>
  </tbody>
</table>

_Featured Albums_
<table>
  <tbody>  
    <tr>
{%- assign latest_type = "updated" -%}
{%- assign latest_updated = site.albums | sort: "date_updated" | reverse %}
{% for album in latest_updated limit:3 -%}
{% include featured.md %}
{% endfor %}
   </tr>
    <tr>
{%- assign latest_type = "featured" -%}
{%- assign new = site.albums | where: "featured", "true" | where: "date_updated", nil | sort: "date" | reverse | limit: 3 -%}
{%- assign updated_size = 3 | minus: new.size -%}
{%- if updated_size > 0 -%}
{%- assign updated = site.albums | where: "featured", "true" | sort: "date_updated" | reverse | limit: updated_size -%}
{%- endif %}
{% for album in new limit:3 -%}
{% include featured.md %}
{% endfor %}
{% for album in updated limit: updated_size -%}
{% include featured.md %}
{% endfor %}
   </tr>
  </tbody>
</table>

![Sax]({% link /assets/images/sax-shadow-1024.jpeg %})



