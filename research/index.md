---
title: "Research"
excerpt: ""
permalink: /research/

# ==============================================================
#  RESEARCH PAGE  —  everything for this page lives in /research
#
#    research/index.md   ← this file: interests + list of papers
#    research/_card.html ← how one paper card looks (rarely edited)
#    research/_style.html← colors and spacing
#
#  HOW TO ADD A PAPER
#    1. Copy one entry below (from "- title:" to its last line).
#    2. Paste it at the TOP of the right section (newest first).
#    3. Change the text. Keep the same indentation.
#
#  FIELDS
#    title     : paper title
#    authors   : author list in order (your name is highlighted automatically)
#    venue     : journal or conference name shown in the badge
#    venue_url : link for the venue badge      (optional)
#    year      : publication year              (optional)
#    paper_url : link for the "Paper" button   (optional)
#    code_url  : link for a "Code" button      (optional)
#    status    : e.g. "Under review" — for works in progress
#
#  To leave an optional field out, delete that line.
# ==============================================================


# ---------------- RESEARCH INTERESTS ----------------
interests:
  - "Reasoning in LLMs: mathematical and multi-step reasoning"
  - "LLM safety and security: prompt injection and jailbreak attacks"
  - "Bias and fairness in large language models"
  - "Multilingual and low-resource LLMs, with a focus on Bengali"
  - "Vision-language models for culturally grounded multimodal content"
  - "LLM evaluation: when to trust LLMs over fine-tuned models"


# ---------------- WORKS IN PROGRESS ----------------
in_progress:

  - title: "Diplomacy Mind: Large Language Models Retrieve Multi-label Geopolitical Topics Associated With Every Single Geographical Region"
    status: "In preparation"

  - title: "Decoding Aggression: A Multi-Level Multimodal Framework for Culturally Grounded Bengali Memes"
    status: "In preparation"

  - title: "When to Ask the LLM: Combining a Fine-Tuned Model and Few-Shot LLMs for Bangla Aspect-Based Sentiment Analysis"
    status: "In preparation"

  - title: "MuTHER: Multilabel Textual Hostility Detection in Social Media Using Ensemble of Transformers"
    status: "Submitted to Applied Soft Computing"


# ---------------- JOURNALS ----------------
journals:

  - title: "TSFC: A Hierarchical Classification Framework for Multimodal Commercial Contents in Bengali"
    authors: "Anik Mahmud Shanto, Fahim Shakil Tamim, Mst. Sanjida Jamal Priya, Mohammed Moshiul Hoque, Enamul Hoque Prince"
    venue: "IEEE Access"
    venue_url: "https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=6287639"
    year: 2026
    paper_url: "https://ieeexplore.ieee.org/abstract/document/11369232/"

  - title: "Enhanced Semantic Relatedness Prediction Using XLM-RoBERTa and CNNs with K-Fold Cross-Validation"
    authors: "Md Ayon Mia, Fahim Shakil Tamim, Zaima Sartaj Taheri, Md Alamin Talukder"
    venue: "The Journal of Engineering"
    venue_url: "https://ietresearch.onlinelibrary.wiley.com/journal/20513305"
    year: 2025
    paper_url: "https://ietresearch.onlinelibrary.wiley.com/doi/full/10.1049/tje2.70106"


# ---------------- CONFERENCES ----------------
conferences:

  - title: "MDC3: A Novel Multimodal Dataset for Commercial Content Classification in Bengali"
    authors: "Anik Mahmud Shanto, Mst. Sanjida Jamal Priya, Fahim Shakil Tamim, Mohammed Moshiul Hoque"
    venue: "NAACL SRW 2025"
    year: 2025
    paper_url: "https://aclanthology.org/2025.naacl-srw.31/"

  - title: "Sentiment Classification of Multi-Modal Memes Using Deep Learning and Transformer Techniques"
    authors: "Tanzin Ahammad, Zaima Sartaj Taheri, Fahim Shakil Tamim"
    venue: "COMPAS 2024"
    year: 2024

  - title: "An Ensemble Approach of Transfer Learning and Vision Transformer to Identify COVID-19 from Chest X-Rays"
    authors: "Fahim Shakil Tamim, Zaima Sartaj Taheri, Sudipta Saha Niloy, Ashim Dey, Annesha Das"
    venue: "ICAEEE 2024"
    year: 2024

  - title: "Detecting Signs of Depression from Social Media Texts Using Generalized Autoregressive Pretraining Transformer Model"
    authors: "Fahim Shakil Tamim, Zaima Sartaj Taheri, Mohammed Moshiul Hoque"
    venue: "ICCIT 2023"
    year: 2023

  - title: "Detecting Violence Inciting Texts Based on Pre-Trained Transformers"
    authors: "Fahim Shakil Tamim, Sourav Saha, Avishek Das, Mohammed Moshiul Hoque"
    venue: "ICCIT 2023"
    year: 2023

  - title: "Optimizing SMS Spam Detection with Large Language Models and Transformer Architectures"
    authors: "Nazir Ahmed, ASM Shakil Ahamed, Fahim Shakil Tamim"
    venue: "ECCE 2023"
    year: 2023
---

{% include_relative _style.html %}

<div class="rs">


<!-- ================= Research interests ================= -->

<p class="rs-lead">
  My research lies in <strong>Natural Language Processing</strong>, with a focus on building
  <strong>trustworthy large language models</strong>. I study how LLMs reason, where they fail,
  and how they can be made safe, fair, and reliable, especially for low-resource languages such as Bengali
  and for culturally grounded multimodal content. My current interests are:
</p>

<ul class="rs-chips">
  {% for item in page.interests %}<li>{{ item }}</li>{% endfor %}
</ul>

<p class="rs-note">
  Social computing topics include hostility, violence, aggression, depression,
  sarcasm, fake news, and sentiment.
</p>


<!-- ================= Publications ================= -->

<h2 class="rs-h">Publications</h2>

<p class="rs-note">
  Full list:
  <a href="https://scholar.google.com/citations?hl=en&amp;user=35u_dC4AAAAJ&amp;view_op=list_works&amp;sortby=pubdate">Google Scholar</a>
  &middot;
  <a href="https://www.semanticscholar.org/author/Fahim-Shakil-Tamim/2287982856">Semantic Scholar</a>
</p>


<h3 class="rs-sub">Works in progress</h3>
{% for pub in page.in_progress %}
  {% include_relative _card.html pub=pub %}
{% endfor %}


<h3 class="rs-sub">Journals</h3>
{% for pub in page.journals %}
  {% include_relative _card.html pub=pub %}
{% endfor %}


<h3 class="rs-sub">Conferences</h3>
{% for pub in page.conferences %}
  {% include_relative _card.html pub=pub %}
{% endfor %}


</div>
