---
layout: single
title: "Blog"
permalink: /blog/
author_profile: true
---

Aqui compartilho análises, reflexões e artigos sobre economia, políticas públicas e temas que acompanho de perto.

---

{% for post in site.posts %}
  {% include archive-single.html %}
{% endfor %}

{% if site.posts.size == 0 %}
*Nenhum post publicado ainda. Em breve, novos conteúdos!*
{% endif %}
