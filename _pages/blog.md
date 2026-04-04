---
layout: archive
title: "Blog"
permalink: /blog/
author_profile: true
---

{% include base_path %}

Aqui compartilho análises, reflexões e artigos sobre economia, políticas públicas e temas que acompanho de perto.

---

{% for post in paginator.posts %}
  {% include archive-single.html %}
{% endfor %}

{% if paginator.total_pages > 1 %}
<div class="pagination">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path | prepend: site.baseurl }}" class="btn btn--primary">← Mais recentes</a>
  {% endif %}
  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path | prepend: site.baseurl }}" class="btn btn--primary">Mais antigas →</a>
  {% endif %}
</div>
{% endif %}
