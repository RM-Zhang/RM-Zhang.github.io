---
layout: archive
title: "Life"
permalink: /life/
author_profile: true
---

{% for post in site.life reversed %}
  <div class="life-entry">
    <h2>{{ post.title }}</h2>
    <p><em>{{ post.date | date: "%Y-%m-%d" }}</em></p>
    {{ post.content | markdownify }}
    <hr>
  </div>
{% endfor %}
