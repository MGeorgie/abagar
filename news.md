---
bg: "abagar3.jpg"
layout: page
title: "News"
crawlertitle: "Activités"
permalink: /news/
summary: "Activités de l'association"
active: news
---

# Activités de L'Association

{% for post in site.posts limit: 5 %}
  <article class="index-page">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {{ post.excerpt }}
  </article>
{% endfor %}
