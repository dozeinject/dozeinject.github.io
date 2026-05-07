---
layout: archive
title: HackTheBox Writeups
permalink: /htb/
---

Welcome to my HackTheBox writeups collection. All machines are organized by difficulty and automatically listed below.

---

{% assign easy = site.categories.htb | where: "difficulty", "Easy" %}
{% assign medium = site.categories.htb | where: "difficulty", "Medium" %}
{% assign hard = site.categories.htb | where: "difficulty", "Hard" %}

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
