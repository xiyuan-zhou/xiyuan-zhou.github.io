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

{% for post in site.publications reversed %}
  <div>
    <div style="display: flex; align-items: center;">
      <img src="{{ post.image }}" alt="{{ post.title }}" style="max-width: 100px; margin-right: 20px;">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    </div>
    <!-- 其他出版物信息，例如作者、日期、链接等 -->
  </div>
  <div style="clear: both;"></div> <!-- 清除浮动以避免样式问题 -->
{% endfor %}
