---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

<ul class="publications-list" style="list-style: none; padding-left: 0;">
{% for post in site.publications reversed %}
  <li style="margin-bottom: 1.2em;">
    <strong>{{ post.title }}</strong><br>
    <span style="color: #555;">{{ post.venue }}, {{ post.date | date: "%Y" }}</span><br>
    {% if post.paperurl %}
      <a href="{{ post.paperurl }}" target="_blank">{{ post.paperurl }}</a>
    {% endif %}
  </li>
{% endfor %}
</ul>
