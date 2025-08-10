---
layout: default
title: Blog
---

<h1>Blog</h1>
<p>Thoughts - some structured, some spontaneous, some random.</p>
{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt | strip_html | truncate: 100 }}</p> <!-- Limits excerpt to 100 characters -->
  </article>
{% endfor %}
