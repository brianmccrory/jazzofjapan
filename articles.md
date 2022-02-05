---
title: Articles
image: /assets/images/J-shaded.jpg
---

# Articles 

{% assign sorted = site.albums | sort_natural: "sort_value" %}
{% for album in sorted -%}
1. [{{ album.artist }}: *{{ album.title }}*]({{ album.url }})
{% endfor %}

---

# Upcoming

1. Bungalow: *Past Life*
1. Hitomi Nishiyama Trio "Parallax": *Live*
1. Kaori Vibes Quartet: *Cross Point*
1. Ken'ichiro Shinzawa: *Piano Works*
1. Manabu Ohishi Trio: *Wish*
1. Mayuko Katakura: *The Echoes of Three*
1. Meu Coracao: *A Tempo*
1. Sanae Ishikawa: *Feel Like Makin' Love*
1. Seiji Endo: *Tsutaete Ikou*
1. Tomoka Miwa: *Colors in Silence*
1. Yuya Wakai: *Images*


---

*Looking for specific musicians, albums, or other terms? [Search this site]({% link search.md %})*
