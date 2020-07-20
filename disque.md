---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
{% for disque in site.posts %}
  <article>
    <h2>
      <!-- <a href="{{ post.url }}"> -->
        {{ disque.title }}
      <!-- </a> -->
    </h2>
  </article>
{% endfor %}