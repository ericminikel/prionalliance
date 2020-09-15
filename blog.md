---
layout: default
title: Blog
---

<div class="home">

  <h1>Posts</h1>

  <ul class="posts">
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a> <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
      </li>
    {% endfor %}
  </ul>

<br>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>

