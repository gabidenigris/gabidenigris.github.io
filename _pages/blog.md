---
layout: archive
title: "Blog"
permalink: /blog/
author_profile: true
---

Aqui compartilho análises, reflexões e artigos sobre economia, políticas públicas e temas que acompanho de perto.

---

{% for post in site.posts %}
  <div class="blog-post-item">
    {% include archive-single.html %}
  </div>
{% endfor %}
