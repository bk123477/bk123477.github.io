---
permalink: /
title: "Minki Hong"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi! I'm Minki Hong. I am currently a Graduate Researcher at **Dongguk University** (M.S. in Computer Science and Artificial Intelligence, advised by Prof. Jihie Kim). Recently, I was a Visiting Scholar at the Bot Intelligence Group (BIG) at **Carnegie Mellon University**, working with Prof. Jean Oh.

My research focuses on developing AI systems that align with human values and understand diverse contexts. Specifically, I am interested in:
- **Generative AI & Social Norms:** Modeling cultural and social contexts for safer dialogue and interaction.
- **Fairness & Inclusivity:** Mitigating cultural and demographic biases in generative models (e.g., image-to-image editing).
- **Reasoning Capabilities:** Eliciting better reasoning in LLMs and VLMs through interpretation grounding and chain-of-thought prompting.

If you would like to connect or chat, please feel free to reach out:

📧 [bk123477@gmail.com](mailto:bk123477@gmail.com) | 
🔗 [LinkedIn](https://www.linkedin.com/in/bk123477) |
📝 [GitHub](https://github.com/bk123477)

---

## 📰 Recent News
<div class="custom-grid-wrapper">
{% assign sorted_posts = site.posts | sort: 'date' | reverse %}
{% for post in sorted_posts limit:2 %}
  {% include archive-single-card.html %}
{% endfor %}
</div>
<div style="text-align: right; margin-top: -10px; margin-bottom: 30px;">
  <a href="{{ '/year-archive/' | relative_url }}"><strong>View all news →</strong></a>
</div>

## 📚 Selected Publications
{% assign sorted_pubs = site.publications | sort: 'date' | reverse %}
{% for post in sorted_pubs limit:3 %}
  {% include archive-single-publication.html %}
{% endfor %}
<div style="text-align: right; margin-top: -10px;">
  <a href="{{ '/publications/' | relative_url }}"><strong>View all publications →</strong></a>
</div>