---
layout: page
title:
permalink: /thoughts/
---

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <h2 class="post-title">
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h2>
      <p class="post-excerpt">{{ post.excerpt }}</p>
      <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    </li>
  {% endfor %}
</ul>
