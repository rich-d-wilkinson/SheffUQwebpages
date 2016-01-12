---
layout: default
title: Sheffield UQ blog
---


# Blog

We'll sporadically post blog entries about things that take our interest, interesting conferences etc.

<ul>  {% for post in site.posts %}
{% if post.categories contains 'blog' %}
    <li>
      <a href="{{ post.url }}">{{post.date | date_to_string}} {{ post.title }}</a>
      <p>
      {{ post.excerpt | remove: '<p>' | remove: '</p>' }}</p>
    </li>
    {% endif %}
  {% endfor %}
</ul>
