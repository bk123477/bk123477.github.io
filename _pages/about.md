---
permalink: /
title: "Minki Hong"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi! I’m Minki Hong, an M.S. student in **Computer Science and Artificial Intelligence** at Dongguk University, advised by Professor Jihie Kim. I received my B.S. degree in **Computer Science & Engineering** from Dongguk University.

My research interests lie in developing AI systems that **align with human social norms and values**. I focus on the intersection of generative AI, **social norms**, and **bias mitigation**, with a particular emphasis on fairness and inclusivity. I am especially fascinated by how cultural and social contexts shape communication and how AI models can better capture these nuances. In addition, I explore methods to **improve the quality of generative AI responses in low-resource environments**, aiming to make AI more accessible and equitable across diverse linguistic and cultural settings.

I am also deeply interested in **eliciting reasoning capabilities in both large language models (LLMs) and vision–language models (VLMs)**. I find it exciting that different prompting and training strategies can enable smaller models to approach the performance of much larger ones, and I am actively exploring methods to bridge this gap.

Currently, I am spending six months as a visiting researcher at the Robotics Institute of Carnegie Mellon University under the supervision of Professor Jean Oh. During this period, I am studying the **interaction between robotics and generative AI**, investigating how these two domains can complement and enrich each other.

If you would like to connect or chat, please feel free to reach out:
📧 [jackyh1@dgu.ac.kr](mailto:jackyh1@dgu.ac.kr) | 
📧 [minkih@andrew.cmu.edu](mailto:minkih@andrew.cmu.edu) | 
🔗 [LinkedIn](https://www.linkedin.com/in/bk123477) |
📝 [My blog](https://velog.io/@jackyh1/posts)


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
- M.S. in Computer Science and Artificial Intelligence. Dongguk University. Mar. 2024 - Present
- B.S. in Computer Science & Engineering. Dongguk University. Mar. 2018 - Feb. 2024