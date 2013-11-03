---
layout: page
title: filsmick's blog
tagline: Make things pretty.
---

{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}  
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p><small><strong>{{ post.date | date: "%B %e, %Y" }}</strong> . {{ post.category }} . <a href="http://erjjones.github.com{{ post.url }}#disqus_thread"></a></small></p>      
  {% endfor %}
</ul>