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
#    selected  : true — also show it under "Selected publications"
#
#  To leave an optional field out, delete that line.
# ==============================================================


# ---------------- RESEARCH INTERESTS ----------------
#   Each interest is a card: a short title and a one-line detail.
interests:
  - title: "Reasoning in LLMs"
    detail: "Mathematical and multi-step reasoning in large language models."
  - title: "Safety and security"
    detail: "Robustness of LLMs against prompt injection and jailbreak attacks."
  - title: "Bias and fairness"
    detail: "Measuring and reducing social bias in what LLMs generate."
  - title: "Multilingual and low-resource NLP"
    detail: "Building and evaluating LLMs for Bengali and other under-served languages."
  - title: "Vision-language models"
    detail: "Understanding culturally grounded multimodal content such as memes."
  - title: "LLM evaluation"
    detail: "Knowing when to trust a general-purpose LLM over a fine-tuned model."


# ---------------- RESEARCH VISION (what you want to study next) ----------------
vision: >-
  I want to understand when large language models can be trusted, and how to make
  them trustworthy for languages and cultures they were not built for. Three questions
  guide my work. How reliably do LLMs reason in low-resource languages such as Bengali,
  and how do their failures differ from those in English? Do safety behaviours, such as
  bias mitigation and defences against jailbreaks and prompt injection, carry over across
  languages and modalities? And when should we rely on a large general-purpose LLM rather
  than a smaller fine-tuned model, and can a system learn to make that choice itself?


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
    selected: true

  - title: "Enhanced Semantic Relatedness Prediction Using XLM-RoBERTa and CNNs with K-Fold Cross-Validation"
    authors: "Md Ayon Mia, Fahim Shakil Tamim, Zaima Sartaj Taheri, Md Alamin Talukder"
    venue: "The Journal of Engineering"
    venue_url: "https://ietresearch.onlinelibrary.wiley.com/journal/20513305"
    year: 2025
    paper_url: "https://ietresearch.onlinelibrary.wiley.com/doi/full/10.1049/tje2.70106"
    selected: true


# ---------------- CONFERENCES ----------------
conferences:

  - title: "MDC3: A Novel Multimodal Dataset for Commercial Content Classification in Bengali"
    authors: "Anik Mahmud Shanto, Mst. Sanjida Jamal Priya, Fahim Shakil Tamim, Mohammed Moshiul Hoque"
    venue: "NAACL SRW 2025"
    year: 2025
    paper_url: "https://aclanthology.org/2025.naacl-srw.31/"
    selected: true

  - title: "Optimizing SMS Spam Detection with Large Language Models and Transformer Architectures"
    authors: "Nazir Ahmed, ASM Shakil Ahamed, Fahim Shakil Tamim"
    venue: "ECCE 2025"
    year: 2025
    paper_url: "https://ieeexplore.ieee.org/document/11013998"

  - title: "Sentiment Classification of Multi-Modal Memes Using Deep Learning and Transformer Techniques"
    authors: "Tanzin Ahammad, Zaima Sartaj Taheri, Fahim Shakil Tamim"
    venue: "COMPAS 2024"
    year: 2024
    paper_url: "https://ieeexplore.ieee.org/document/10796143"

  - title: "An Ensemble Approach of Transfer Learning and Vision Transformer to Identify COVID-19 from Chest X-Rays"
    authors: "Fahim Shakil Tamim, Zaima Sartaj Taheri, Sudipta Saha Niloy, Ashim Dey, Annesha Das"
    venue: "ICAEEE 2024"
    year: 2024
    paper_url: "https://ieeexplore.ieee.org/document/10561636"

  - title: "Detecting Signs of Depression from Social Media Texts Using Generalized Autoregressive Pretraining Transformer Model"
    authors: "Fahim Shakil Tamim, Zaima Sartaj Taheri, Mohammed Moshiul Hoque"
    venue: "ICCIT 2023"
    year: 2023
    paper_url: "https://ieeexplore.ieee.org/document/10441486"

  - title: "Detecting Violence Inciting Texts Based on Pre-Trained Transformers"
    authors: "Fahim Shakil Tamim, Sourav Saha, Avishek Das, Mohammed Moshiul Hoque"
    venue: "ICCIT 2023"
    year: 2023
    paper_url: "https://ieeexplore.ieee.org/document/10441268"
    selected: true

---

{% include_relative _style.html %}

<div class="rs">


<!-- ================= Research interests ================= -->

<p class="rs-lead">
  My research is in <strong>Natural Language Processing</strong>, centred on
  <strong>trustworthy large language models</strong>. I study how LLMs reason, where and why they fail,
  and how to make them safe, fair, and reliable, particularly for low-resource languages such as Bengali
  and for culturally grounded multimodal content. My current interests are:
</p>

<div class="rs-interests">
  {% for item in page.interests %}
  <div class="rs-interest">
    <span class="rs-interest-title">{{ item.title }}</span>
    <span class="rs-interest-detail">{{ item.detail }}</span>
  </div>
  {% endfor %}
</div>

<p class="rs-note">
  Social computing topics include hostility, violence, aggression, depression,
  sarcasm, fake news, and sentiment.
</p>


<!-- ================= Research vision ================= -->

{% if page.vision %}
<h2 class="rs-h">Research vision</h2>
<p class="rs-lead rs-vision">{{ page.vision }}</p>
{% endif %}


<!-- ================= Publications ================= -->

<h2 class="rs-h">Publications</h2>

<p class="rs-note">
  Full list:
  <a href="https://scholar.google.com/citations?hl=en&amp;user=35u_dC4AAAAJ&amp;view_op=list_works&amp;sortby=pubdate">Google Scholar</a>
  &middot;
  <a href="https://www.semanticscholar.org/author/Fahim-Shakil-Tamim/2287982856">Semantic Scholar</a>
</p>


{% assign all_pubs = page.journals | concat: page.conferences %}
{% assign selected = all_pubs | where: "selected", true %}
{% if selected.size > 0 %}
<h3 class="rs-sub">Selected publications</h3>
{% for pub in selected %}
  {% include_relative _card.html pub=pub %}
{% endfor %}
{% endif %}


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
