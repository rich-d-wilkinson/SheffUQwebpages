---
layout: default
title: Sheffield UQ events
---


# Events

We'll list forthcoming and past events here.

<h1>2017</h1>
<ul class="posts">
{% for post in site.posts %}
    {% if post.categories contains 'events' %}
    {% capture year %}{{post.date | date: "%Y"}}{% endcapture %}
  {% if year == "2017" %}
        <li>
        <a href="{{ post.url }}">{{post.date | date_to_string}} {{ post.title }}</a>
        <p>
        {{ post.excerpt | remove: '<p>' | remove: '</p>' }}</p>
        </li>
    {% endif %}
    {% endif %}
{% endfor %}
</ul>

<h1>2016</h1>
<ul class="posts">
{% for post in site.posts %}
    {% if post.categories contains 'events' %}
    {% capture year %}{{post.date | date: "%Y"}}{% endcapture %}
  {% if year == "2016" %}
        <li>
        <a href="{{ post.url }}">{{post.date | date_to_string}} {{ post.title }}</a>
        <p>
        {{ post.excerpt | remove: '<p>' | remove: '</p>' }}</p>
        </li>
    {% endif %}
    {% endif %}
{% endfor %}
</ul>

<h1>2015</h1>
<ul class="posts">
{% for post in site.posts %}
    {% if post.categories contains 'events' %}
    {% capture year %}{{post.date | date: "%Y"}}{% endcapture %}
  {% if year == "2015" %}
        <li>
        <a href="{{ post.url }}">{{post.date | date_to_string}} {{ post.title }}</a>
        <p>
        {{ post.excerpt | remove: '<p>' | remove: '</p>' }}</p>
        </li>
    {% endif %}
    {% endif %}
{% endfor %}
</ul>