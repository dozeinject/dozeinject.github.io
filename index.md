---
layout: default
title: DozeInject Blog
---

# DozeInject Blog

Cybersecurity notes, web hacking labs, networking fundamentals and CTF writeups.

---

## 📌 Recent Posts

<ul>
{% for post in site.posts limit:5 %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <small>— {{ post.date | date: "%Y-%m-%d" }}</small>
  </li>
{% endfor %}
</ul>

---

## 📚 Topics

- Web Security (XSS, SQLi, SSRF, etc.)
- Networking (TCP/IP, Ethernet, STP)
- CTF Writeups (HackTheBox, PortSwigger, Root-Me)

---

## About

Exploring cybersecurity through hands-on labs and structured notes.
