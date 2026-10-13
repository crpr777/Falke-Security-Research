---
layout: page
title: Archive
permalink: /archive/
lead: Posts grouped by the three research topics.
---

{% for topic in site.topics %}
<section class="archive-topic" id="{{ topic | slugify }}">
  <h2>{{ topic }}</h2>
  {% assign found = false %}
  <ol class="archive-list">
    {% for post in site.posts %}
      {% if post.categories contains topic %}
        {% assign found = true %}
        <li>
          <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y-%m-%d" }}</time>
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </li>
      {% endif %}
    {% endfor %}
  </ol>
  {% unless found %}
    <p class="muted">No posts in this topic yet.</p>
  {% endunless %}
</section>
{% endfor %}
