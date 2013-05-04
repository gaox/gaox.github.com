---
layout: page
title: Some random stuff
tagline: 
---
{% include JB/setup %}

{% for post in site.posts offset: 0 limit: 6 %}
  <div id="entry-post">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p class="meta">
        <time datetime="{{ post.date }}">{{ post.date | date: "%B %d, %Y" }}</time>
      </p>
      {{ post.content }}
  </div>
{% endfor %}
