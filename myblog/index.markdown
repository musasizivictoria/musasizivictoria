---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: "Style Meets Substance"
---

Welcome to Victoria Musasizi's fashion blog, where design meets education. Explore my posts below to learn more about my journey as a fashion designer and educator.

{% for post in site.posts %}
<div class="post-preview">
  <h2>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </h2>
  <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
  <p>{{ post.excerpt }}</p>
  <a href="{{ post.url | relative_url }}">Read more...</a>
</div>
{% endfor %}
