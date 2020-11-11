---
layout: default
---
<article>
<span class="title">Disque</span>
<img class="main-image" src="{{ page.image | relative_url }}" />
<span class="subtitle">{{ page.artist }}</span>
<h1>{{ page.title }}</h1>
<div class="content">{{ content }}</div>
<section id="others">
  <h2>Autres sorties</h2>
  <div id="last-albums">
  {% assign disques = site.disques | where_exp:"disque","disque.url != page.url" %}
  {% for disque in disques limit:3 %}
    <a href="{{ disque.url | relative_url }}">
      <img src="{{ disque.thumbnail | relative_url }}" />
      <h3>{{ disque.title }}</h3>
      <h4 class="artist">{{ disque.artist }}</h4>
    </a>
  {% endfor %}
  </div>
  <a class="see-more" href="{{ '/disque' | relative_url }}">Voir tous les disques</a>
</section>