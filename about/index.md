---
title: "Hello, I'm Tamim"
excerpt: "About me"
author_profile: true
permalink: /
redirect_from:
  - /about/
  - /about.html

# ==============================================================
#  HOME PAGE  -  everything for this page lives in /about
#
#    about/index.md    <- this file: intro, links and news
#    about/_style.html <- colors and spacing
#
#  HOW TO ADD A NEWS ITEM
#    Copy one entry under "news:", paste it at the TOP, and edit.
#    The text can contain links:  <a href="https://...">text</a>
# ==============================================================


# ---------------- TAGLINES (typed one by one above the title) ----------------
taglines:
  - "NLP researcher building reliable LLMs for Bengali."
  - "Probing LLMs for bias, reasoning, and jailbreaks."
  - "Lecturer in Computer Science and Engineering at IUBAT."
  - "Exploring when to trust LLMs over fine-tuned models."
  - "Teaching machines to understand culturally grounded content."
  - "Working on multimodal, multilingual, and socially grounded NLP."


# ---------------- QUICK LINKS (buttons under the intro) ----------------
links:
  - label: "Email"
    url: "mailto:fstamim9@gmail.com"
  - label: "Resume"
    url: "https://drive.google.com/file/d/1KLxo9yFKQuzWY8fA57siI1U1rK7ZLMEG/view?usp=sharing"
  - label: "Google Scholar"
    url: "https://scholar.google.com/citations?hl=en&user=35u_dC4AAAAJ&view_op=list_works&sortby=pubdate"
  - label: "GitHub"
    url: "https://github.com/FS-Tamim"


# ---------------- RESEARCH FOCUS (tags) ----------------
focus:
  - "Reasoning in LLMs"
  - "LLM safety and jailbreaks"
  - "Bias and fairness"
  - "Multilingual and Bengali NLP"
  - "Vision-language models"


# ---------------- NEWS (newest first) ----------------
news:

  - date: "Jan 2026"
    text: 'One <a href="https://ieeexplore.ieee.org/document/11369232">paper</a> published in <a href="https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=6287639">IEEE Access</a> (Impact Factor 3.6, CiteScore 9).'

  - date: "Dec 2025"
    text: 'Four papers accepted at <a href="https://iccit.org.bd/2025/home/">ICCIT 2025</a>.'

  - date: "Jan 2024"
    text: 'Joined <a href="https://iubat.edu">IUBAT</a> as a Lecturer in the Department of CSE.'
---

{% include_relative _style.html %}
{% include_relative _tagline.html %}

<div class="ab">


<!-- ================= Intro ================= -->

<p class="ab-lead">
  I am a <strong>Lecturer</strong> in the Department of Computer Science and Engineering at
  <a href="https://iubat.edu/">International University of Business Agriculture and Technology (IUBAT)</a>,
  and a research fellow at the
  <a href="https://www.researchgate.net/lab/CUET-NLP-Lab-Moshiul-Hoque">CUET NLP Lab</a>.
  My research focuses on building <strong>trustworthy large language models</strong>: how they reason,
  where they fail, and how to make them safe and fair, especially for low-resource languages such as Bengali.
  I work on mathematical reasoning, bias, prompt injection and jailbreak attacks, and vision-language models
  for culturally grounded content.
</p>

<p class="ab-text">
  I completed my B.Sc. in Computer Science and Engineering at CUET, where I joined the CUET NLP Lab in my junior years
  and continue to collaborate today. Under the supervision of
  <a href="https://scholar.google.com/citations?user=srYxYhcAAAAJ&amp;hl=en">Prof. Mohammed Moshiul Hoque</a>,
  I built Bengali NLP datasets, published in peer-reviewed venues, and completed my thesis on textual hostility detection
  in social media using ensemble transformer models. Beyond research, I took part in shared tasks and hackathons and served as
  General Secretary of the CUET Computer Club and Organizing Secretary of CUET CSE Fest.
</p>

<p class="ab-text">
  At IUBAT, I have taught core CSE courses for the past two years. I aim to create an inclusive, supportive learning environment
  and actively mentor students to help them grow academically and professionally.
</p>

<div class="ab-focus">
  {% for f in page.focus %}<span class="ab-chip">{{ f }}</span>{% endfor %}
  <a class="ab-more" href="{{ '/research/' | relative_url }}">See my research &rarr;</a>
</div>

<div class="ab-links">
  {% for l in page.links %}<a class="ab-btn {% if forloop.first %}primary{% endif %}" href="{{ l.url }}">{{ l.label }}</a>{% endfor %}
</div>


<!-- ================= News ================= -->

<h2 class="ab-h">News</h2>

<ul class="ab-news {% if page.news.size > 8 %}scroll{% endif %}">
  {% for n in page.news %}
  <li>
    <span class="ab-date">{{ n.date }}</span>
    <span class="ab-item">{{ n.text }}</span>
  </li>
  {% endfor %}
</ul>


</div>
