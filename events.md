---
layout: default
title: Sheffield UQ events
---


# Events

We'll list forthcoming and past events here.

<ul class="posts">
{% for post in site.posts %}
    {% if post.categories contains 'events' %}
        <li>
        <a href="{{ post.url }}">{{post.date | date_to_string}} {{ post.title }}</a>
        <p>
        {{ post.excerpt | remove: '<p>' | remove: '</p>' }}</p>
        </li>
    {% endif %}
{% endfor %}
</ul>
