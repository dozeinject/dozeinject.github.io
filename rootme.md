---
layout: archive
title: Root-Me Writeups
permalink: /rootme/
---

# Root-Me Writeups

Welcome to my Root-Me challenges collection. All challenges are organized by difficulty and automatically listed below.

---

{% assign easy = site.categories.rootme | where: "difficulty", "Easy" %}
{% assign medium = site.categories.rootme | where: "difficulty", "Medium" %}
{% assign hard = site.categories.rootme | where: "difficulty", "Hard" %}

{% if easy.size > 0 %}
## Difficulty: Easy
{% for post in easy %}
- [{{ post.title }}]({{ post.url }}){% if post.excerpt %} – {{ post.excerpt }}{% endif %}
{% endfor %}
{% endif %}

{% if medium.size > 0 %}
## Difficulty: Medium
{% for post in medium %}
- [{{ post.title }}]({{ post.url }}){% if post.excerpt %} – {{ post.excerpt }}{% endif %}
{% endfor %}
{% endif %}

{% if hard.size > 0 %}
## Difficulty: Hard
{% for post in hard %}
- [{{ post.title }}]({{ post.url }}){% if post.excerpt %} – {{ post.excerpt }}{% endif %}
{% endfor %}
{% endif %}
