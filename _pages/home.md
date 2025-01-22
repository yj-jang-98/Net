---
permalink: /
title: "Home"
author_profile: false
redirect_from: 
  - /home/
  - /home.html
---

Takashi Tanaka
---
<img src="/images/tanaka-199x300.jpg#left" width="25%">

Associate Professor

Office: ARMS 2037

Office Phone: +1 765-494-5143

E-mail: tanaka16@purdue.edu

[Research](/research/)

[Publications](/publications/)

News
---
<ul>
  {% for post in site.posts limit:3 %}
    {% if post.categories contains "news" %}
      <li>
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p>{{ post.date | date: "%Y-%m-%d" }}</p>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endif %}
  {% endfor %}
</ul>