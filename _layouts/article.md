---
layout: default
---
<article>
<span class="title">Actualité</span>
{% if page.introVideo %}
<div class="embed" style="padding-bottom: calc((100 / 560) * 315%); margin-bottom: 2rem"><iframe width="560" height="315" src="{{ page.introVideo }}" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>
{% endif %}
<span class="subtitle">{{ page.artist }}</span>
<h1>{{ page.title }}</h1>
<div class="content">{{ content }}</div>