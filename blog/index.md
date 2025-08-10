---
layout: default
title: Blog
---

<h1>Blog</h1>
<p>Thoughts - some structured, some spontaneous, some random.</p>
{% for post in site.posts %}
  <article>
    <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt | strip_html | truncate: 100 }}</p>
  </article>
{% endfor %}
