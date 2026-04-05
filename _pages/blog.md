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
  <h3 class="blog-post-title"><a href="{{ post.url }}">{{ post.title }}</a></h3>
  {% if post.subtitle %}<p class="blog-post-subtitle">{{ post.subtitle }}</p>{% endif %}
  <p class="blog-post-meta">
    {% if post.source_url and post.source_name %}
      Publicado em <a href="{{ post.source_url }}" target="_blank">{{ post.source_name }}</a> &middot;
    {% endif %}
    {{ post.date | date: "%d/%m/%Y" }}
  </p>
</div>
{% endfor %}
