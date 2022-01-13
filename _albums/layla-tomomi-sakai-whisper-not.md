---
layout: default
title: Whisper Not
artist: Layla Tomomi Sakai
year: 1999
cover: layla-tomomi-sakai-whisper.jpeg
---


# {{ site.data.layla-tomomi-sakai-whisper-not.artist }}: {{ site.data.layla-tomomi-sakai-whisper-not.title }}


<p align="center">
<img src="/assets/images/{{ site.data.layla-tomomi-sakai-whisper-not.cover }}">
</p>

<em>Whisper Not</em> is vocalist Layla Tomomi Sakai’s debut release from 2016. Performing here with an intimate guitar and trumpet combo, the striking singer chooses comfortable jazz standards such as “Black Coffee”, “I Can’t Get Started”, and “There Will Never Be Another You” to introduce new listeners to her smooth, husky voice and relaxing style. Six songs are included, and tempos settle at midtempo swing, bluesy groove, or slow sultry ballads, with energy peaking on the quick and exciting “Devil May Care”.

Buoyed by guitar chords and trumpet improvisation, Sakai’s voice emotes cleanly with a strong, whispering texture. She delivers lyrics with a romantic sincerity and gentle confidence, enticing with subtle mystery like a sly wink given with a sweet smile. Each of the songs clocks in at under five minutes and the album is a quick 25-minute play, a pleasurable coffeehouse break or dreamy escape.



<ul>
{% for member in site.data.layla-tomomi-sakai-whisper-not.members %}
<li>
{% if member.url %}<a href="{{ member.url }}">{% endif %}
{{ member.name }}
{% if member.url %}</a>{% endif %}
 - {{ member.instrument }}</li>
{% endfor %}
</ul>

Released in {{ site.data.layla-tomomi-sakai-whisper-not.year }} on {{ site.data.layla-tomomi-sakai-whisper-not.label }} as {{ site.data.layla-tomomi-sakai-whisper-not.code }}.

<em>(Names in Japanese:</em>
{% for m in site.data.layla-tomomi-sakai-whisper-not.members -%}
<em>{{ m.name -}}&nbsp;{{ m.japanese_name -}}</em>
{% endfor -%})



{% for i in site.data.layla-tomomi-sakai-whisper-not.images %}
<img src="/assets/images/{{ i }}">
{% endfor %}

Videos:
<ul>
{% for video in site.data.layla-tomomi-sakai-whisper-not.videos %}
<li><a href="{{ video.url }}">{{ video.comment }}</a></li>
{% endfor %}
</ul>
