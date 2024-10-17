---
layout: page
title: Teaching
permalink: teaching/
---

Academic courses










<div class="posts">
  {% for post in site.categories.teaching limit:10 %}
  <article class="post">
    <h2 class="post-title">
      <a href="{{ site.baseurl }}{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>

    <time datetime="{{ post.date | date: "%B %-d, %Y" }}" class="post-date">{{ post.date | date: "%B %-d, %Y" }}</time>

    {{ post.excerpt }}
  </article>
  {% endfor %}
</div>








