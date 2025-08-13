---
layout: page
title:
permalink: /thoughts/
---

<ul class="post-list">
  {% for post in site.posts %}
    <li class="post-list__item">
      <h2 class="post__title">
        <a class="post__link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h2>
      <p class="post__excerpt">{{ post.excerpt }}</p>
      <p class="post__meta">{{ post.date | date: "%B %d, %Y" }}</p>
    </li>
  {% endfor %}
</ul>
