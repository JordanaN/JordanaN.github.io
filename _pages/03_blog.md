---

layout: blog
title: Blog
permalink: /blog/
---

{% for post in site.posts %}
<ul>
  <li>
    <time>{{ post.date | date: "%b %-d, %Y" }}</time>
    <h3><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
  </li>
</ul>
{% endfor %}
