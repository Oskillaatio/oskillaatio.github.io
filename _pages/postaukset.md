---
permalink: /postaukset/
title: "Kaikki postaukset"
toc: false
toc_label: "Listaus"
toc_sticky: true
---

{% for post in site.posts %}
  <article>
    <h2>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <b><time datetime="{{ post.date | date: "%d.%m.%Y"" }}">{{post.date | date: "%d.%m.%Y"}}</time></b>
    {{ post.excerpt | markdownify }}
    {% for tag in post.tags %}
        <a href="{{/tags/#" tag}}" class="page__taxonomy-item p-category" rel="tag">{{tag}}</a>
    {% endfor %}
  </article>
{% endfor %}