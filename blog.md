---
layout: default
title: Blog
---

{% include JB/setup %}

<div class="home">
  
  <ul class="posts" style="list-style-type:none;">
    {% for post in site.posts %}
      <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        {{ post.excerpt }}
        <br>
      </li>
      <br>
    {% endfor %}
  </ul>

</div>
