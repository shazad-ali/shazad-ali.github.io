---
layout: page
title: Blog
permalink: /blog/
---

<h1 class="subheader">All Posts</h1>
<ul class="no-bullet">
  {% for post in site.posts %}
    <li>
      <h3>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h3>
      <span  class="label">{{ post.date | date: "%b %-d, %Y" }}</span>
    </li>
  {% endfor %}
</ul>
