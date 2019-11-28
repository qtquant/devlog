---
layout: default
title: "开发日志"
---
## {{ page.title }}

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ site.baseurl}}{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>