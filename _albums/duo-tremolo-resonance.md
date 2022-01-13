---
layout: default
title: Resonance
artist: Duo Tremolo
year: 2019
cover: duo-tremolo-resonance.jpeg
---


# {{ site.data.duo-tremolo-resonance.artist }}: {{ site.data.duo-tremolo-resonance.title }}


<p align="center">
<img src="/assets/images/{{ site.data.duo-tremolo-resonance.cover }}">
</p>

Pianist Hideaki Hori and guitarist Takayoshi Baba create beautiful music together on <em>Resonance</em>, their first studio recording as the unit “Duo Tremolo”. On eleven tracks made up of four standards and seven original compositions, the pair play through easy-going swing, bop, and jazz/rock tracks with hues of Jarrett, Corea, and Metheney glowing within.

The graceful players combine the dimensions of Hori’s precise, finessed notes and Baba’s snazzy, bluesy lines at relaxed mid-tempo jaunts, rapid and fluid modern pieces, Latin grooves, and gentle ballads. The music is joyful and emotive, and the two converse with a comfortable flow built solidly on their years performing in various settings. The duo clearly enjoys playing together and it comes through in their playful, professional music.

Two of the songs also feature guest percussionist Saori Sendo, and add rich rhythms and dynamics on Bob Berg’s “Friday Night at the Cadillac Club” and Baba’s “J.M.”. The final track “Pedra Bonita” adds another successful layer, where the two musicians are joined by singer Aya Kurosawa on the grooving Brazilian celebration with a rousing vocal ending.



<ul>
{% for member in site.data.duo-tremolo-resonance.members %}
<li>
{% if member.url %}<a href="{{ member.url }}">{% endif %}
{{ member.name }}
{% if member.url %}</a>{% endif %}
 - {{ member.instrument }}</li>
{% endfor %}
</ul>

Released in {{ site.data.duo-tremolo-resonance.year }} on {{ site.data.duo-tremolo-resonance.label }} as {{ site.data.duo-tremolo-resonance.code }}.

<em>(Names in Japanese:</em>
{% for m in site.data.duo-tremolo-resonance.members -%}
<em>{{ m.name -}}&nbsp;{{ m.japanese_name -}}</em>
{% endfor -%})



{% for i in site.data.duo-tremolo-resonance.images %}
<img src="/assets/images/{{ i }}">
{% endfor %}

Videos:
<ul>
{% for video in site.data.duo-tremolo-resonance.videos %}
<li><a href="{{ video.url }}">{{ video.comment }}</a></li>
{% endfor %}
</ul>
