---
permalink: /about/
title: "About"
author_profile: true
redirect_from:
  - /about.html
---

I am a second-year Ph.D. candidate in Computer Science at the [HKUST NLP Group](https://nlp.ust.hk/), advised by Professor Junxian He. I received my B.Eng. in Automation (IEEE Honor Class) from Shanghai Jiao Tong University in 2024.

My research focuses on natural language processing and machine learning. I am broadly interested in building trustworthy and capable reasoning systems.

## Research interests and skills

- Agentic large language models and long-horizon reasoning
- Logical reasoning and reinforcement learning
- Vision-language models and perception bottlenecks
- LLM truthfulness, hallucination mitigation, and interpretability
- Large-scale verifiable data synthesis and model evaluation

## Research experience

- **Research Intern, Apple MLR, Cupertino** (April 2026–present), mentored by Yizhe Zhang
- **Research Intern, MiniMax** (February 2025–2026), contributing to the M1 and M2.x models and large-scale logical-reasoning data synthesis
- **Research Intern, Tencent WXG** (June–September 2024)
- **Research Intern, Shanghai AI Lab** (June–December 2023)

## Education

- **Ph.D. in Computer Science**, Hong Kong University of Science and Technology, 2024–present
- **B.Eng. in Automation (IEEE Honor Class)**, Shanghai Jiao Tong University, 2020–2024
  - Recipient of the Zhiyuan Honor Scholarship

## Publications

{% include base_path %}

{% if site.publication_category %}
  {% for category in site.publication_category %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h3>{{ category[1].title }}</h3><hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}

[View the dedicated Publications page]({{ base_path }}/publications/).

## Contact

- Email: [jliugi@connect.ust.hk](mailto:jliugi@connect.ust.hk)
- GitHub: [Vicent0205](https://github.com/Vicent0205)
- [Google Scholar](https://scholar.google.com/citations?user=tbK9jl4AAAAJ&hl=en)
- X: [@junteng88716710](https://x.com/junteng88716710)
