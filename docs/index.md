---
layout: default
---

{%- assign date_format = site.minima.date_format | default: "%Y/%m/%d" -%}

<ul>
  {% for post in site.posts %}
    <li>
      <span>{{ post.date | date: date_format }}</span>
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
      <a href="/GithubPages-Test{{ post.url }}">{{ post.title }}</a>
      <a href="{{ site.baseurl }}/{{ post.url }}">{{ post.title }}</a>
      <a href="/GithubPages-Test/{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
