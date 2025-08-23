---
permalink: /
title: "Academic Pages is a ready-to-fork GitHub Pages template for academic personal websites"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

안녕하세요! (자기소개 2~3문장)

## 📰 News
{% assign sorted_posts = site.posts | sort: 'date' | reverse %}
<ul>
{% for post in sorted_posts limit:5 %}
  <li>
    <strong>{{ post.date | date: "%b %d, %Y" }}</strong> – 
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
<p><a href="{{ '/year-archive/' | relative_url }}">More →</a></p>

## 📚 Publications
{% assign sorted_pubs = site.publications | sort: 'year' | reverse %}
<ul>
{% for p in sorted_pubs limit:5 %}
  <li>
    {% if p.venue %}<span>{{ p.venue }} {{ p.year }}</span> — {% endif %}
    <a href="{{ p.url | relative_url }}">{{ p.title }}</a>
    {% if p.authors %}<br/><small>{{ p.authors }}</small>{% endif %}
    {% if p.pdf %} · <a href="{{ p.pdf }}">PDF</a>{% endif %}
  </li>
{% endfor %}
</ul>
<p><a href="{{ '/publications/' | relative_url }}">All publications →</a></p>

## 🎓 Education
- 2024– : M.S., Dongguk University (…)
- 2020–2024: B.S., CSE, Dongguk University (…)