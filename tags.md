---
layout: default
title: Tags
permalink: /tags/
---

<h1 class="post-title">Tags</h1>

<div class="tags-index">
{% assign all_tags = site.posts | map: "tags" | join: "," | split: "," | uniq | sort %}
{% for tag in all_tags %}
  {% assign tag_posts = site.posts | where_exp: "post", "post.tags contains tag" %}
  <div class="tag-group">
    <a href="/tags/{{ tag | slugify }}/" class="tag-heading">
      <span class="tagchip">{{ tag }}</span>
      <span class="tag-count">{{ tag_posts.size }} post{% if tag_posts.size != 1 %}s{% endif %}</span>
    </a>
  </div>
{% endfor %}
</div>
