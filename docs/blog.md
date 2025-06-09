---
layout: archive
title: "Blog"
permalink: /blog/
entries_layout: horizontal
---

{% assign posts = site.posts %}
{% for post in posts %}
  {% include archive-single.html type="horizontal" %}
{% endfor %}
