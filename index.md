---
layout: default
title: Accueil
ordre: 1
---

<ul>
  {% for post in site.posts reversed offset:2 limit:3 %}
    <li>
      <a class="titreArticle" href="{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

<ul>
    {% for file in site.cours %}
        <li>
            <h3>{{ file.title }}</h3>
        </li>
    {% endfor %}
</ul>

