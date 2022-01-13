---
layout: default
title: Madrigal
artist: Chihiro Yamanaka Trio
year: 2004
cover: chihiroyamanaka-madrigal.jpeg
---


# {{ site.data.chihiro-yamanaka-trio-madrigal.artist }}: {{ site.data.chihiro-yamanaka-trio-madrigal.title }}


<p align="center">
<img src="/assets/images/{{ site.data.chihiro-yamanaka-trio-madrigal.cover }}">
</p>

On her third album Madrigal, jazz pianist Chihiro Yamanaka continues on her upward arc, working her magic on jazz standards and originals with a top-notch trio.

With momentum built from her debut Living Without Friday (2001) and When October Goes (2002), on Madrigal (2004), the pianist impresses with new arrangements, tight playing, and flashy piano solos. Recorded in studio with a great live sound, Yamanaka is backed by quality rhythm section mates bassist Larry Grenadier and drummer Jeff Ballard (stalwart members of Brad Mehldau’s trio), and drummer Rodney Green on three tracks.

This is her third album on the boutique Osaka-based Atelier Sawano label. With nine tracks, the album clocks in at a brisk 47 minutes of pure jazz fun. This album completes her early Atelier Sawano trilogy, a great introduction to Yamanaka’s jazz skills and vision which she would continue to pursue on releases for major labels Verve and Blue Note.

As on her prior two albums, the music on Madrigal showcases her dexterous threads of improvised notes flowing with a clean touch. Yamanaka also spins her distinctively original arrangements of classic jazz tunes (“Caravan”, “Take Five”), a welcome touchstone on previous and future recordings as well. Compared to her earlier releases, Madrigal shoots for perhaps an even more kinetic mood, with boundless energy and an acrobatic spirit displayed. In fact, Yamanaka dedicated this album to her childhood, and the music is infused with playful creativity as suggested by the album photos and liner notes.

A track-by-track rundown: simply swinging on “Antonio’s Joke”, addictively fun “Living Time Event V”, the pretty, light “Madrigal”, the unbridled “Ojos De Rojo”, a scrambling “School Days”, the quick Brazilian “Salve Salgueiro”, a strong and distinctive “Caravan”, the cute “Lesson 51”, and a reworked, shifting “Take Five”. Most songs are midtempo or faster, the energy undepletable. The first and third tracks are originals from the pianist, while the cover songs were written by George Russell, Cedar Walton, Duke Ellington, Paul Desmond, and other greats.

<ul>
{% for member in site.data.chihiro-yamanaka-trio-madrigal.members %}
<li>
{% if member.url %}<a href="{{ member.url }}">{% endif %}
{{ member.name }}
{% if member.url %}</a>{% endif %}
 - {{ member.instrument }}</li>
{% endfor %}
</ul>

Released in {{ site.data.chihiro-yamanaka-trio-madrigal.year }} on {{ site.data.chihiro-yamanaka-trio-madrigal.label }} as {{ site.data.chihiro-yamanaka-trio-madrigal.code }}.

<em>(Names in Japanese:</em>
{% for m in site.data.chihiro-yamanaka-trio-madrigal.members -%}
<em>{{ m.name -}}&nbsp;{{ m.japanese_name -}}</em>
{% endfor -%})



{% for i in site.data.chihiro-yamanaka-trio-madrigal.images %}
<img src="/assets/images/{{ i }}">
{% endfor %}

Videos:
<ul>
{% for video in site.data.chihiro-yamanaka-trio-madrigal.videos %}
<li><a href="{{ video.url }}">{{ video.comment }}</a></li>
{% endfor %}
</ul>
