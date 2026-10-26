---
title: "Education & Experience"
excerpt: ""
author_profile: true
permalink: /education/

# ==============================================================
#  EDUCATION & EXPERIENCE PAGE  -  everything lives in /education
#
#    education/index.md    <- this file: all the content
#    education/_style.html <- colors and spacing
#
#  To add an entry, copy one block (from "- title:" to its last
#  line), paste it at the TOP of the right section, and edit it.
#  Keep the same indentation. Delete any line you don't need.
#
#  FIELDS
#    title    : university / company / course name
#    subtitle : degree / job title
#    period   : e.g. "2018 - 2023"
#    location : city, country               (optional)
#    url      : website link for the title  (optional)
#    facts    : short highlighted items, e.g. CGPA, position
#    points   : bullet points
#    status   : e.g. "Completed" or "In progress" (certifications)
# ==============================================================


# ---------------- EDUCATION ----------------
education:

  - title: "Chittagong University of Engineering and Technology (CUET)"
    url: "https://www.cuet.ac.bd/"
    subtitle: "B.Sc. in Computer Science and Engineering"
    period: "2018 - 2023"
    location: "Chittagong, Bangladesh"
    facts:
      - "CGPA 3.79 / 4.00 (with honors)"
      - "Position 9th / 126"
      - "Dean's Award"
    points:
      - 'Advisor: <a href="https://scholar.google.com/citations?hl=en&amp;user=srYxYhcAAAAJ&amp;view_op=list_works&amp;sortby=pubdate">Prof. Mohammed Moshiul Hoque</a>'

  - title: "Notre Dame College"
    subtitle: "Higher Secondary Certificate (HSC)"
    period: "2015 - 2017"
    location: "Dhaka, Bangladesh"
    facts:
      - "GPA 5.00 / 5.00"
      - "Talent Pool Scholarship, Dhaka Board"

  - title: "Dhaka Residential Model College"
    subtitle: "Secondary School Certificate (SSC)"
    period: "2013 - 2015"
    location: "Dhaka, Bangladesh"
    facts:
      - "GPA 5.00 / 5.00"


# ---------------- WORK EXPERIENCE ----------------
experience:

  - title: "International University of Business Agriculture and Technology (IUBAT)"
    url: "https://iubat.edu/"
    subtitle: "Lecturer, Department of Computer Science and Engineering"
    period: "Jan 2024 - Present"
    location: "Dhaka, Bangladesh"
    points:
      - "Deliver undergraduate CSE courses and provide academic consultation and mentorship following the Outcome-Based Education (OBE) framework."
      - "Supervise thesis and practicum students in research methodology, project management, and academic writing, applying Continuous Quality Improvement (CQI) practices."
      - "Design and implement curriculum improvements that strengthen learning outcomes and student engagement."

  - title: "CUET NLP Lab"
    subtitle: "Research Fellow"
    period: "Feb 2022 - Present"
    location: "Chittagong, Bangladesh"
    points:
      - "Develop benchmark Bengali datasets and publish research that advances low-resource NLP."
      - "Explore large language models, multimodal systems, and generative NLP, contributing to publications in these areas."
      - "Participate in shared-task competitions and mentor junior researchers in NLP, ML, and DL."

  - title: "Robi Axiata Limited | Red Dot Digital"
    subtitle: "Industrial Attachment Trainee"
    period: "Oct 2022 - Nov 2022"
    location: "Dhaka, Bangladesh"
    points:
      - "Worked with production platforms including the My Robi app, Binge, CRM, HRMS, SIM registration, and MFS."
      - "Gained hands-on experience in software workflows, teamwork, and professional communication."


# ---------------- CERTIFICATIONS ----------------
certifications:

  - title: "Deep Learning Specialization"
    subtitle: "DeepLearning.AI (Coursera)"
    status: "Completed"
    points:
      - "Foundations of deep learning: CNNs, RNNs, LSTMs, optimization (Adam, Dropout, BatchNorm, Xavier/He initialization), and hyper-parameter tuning."
      - "Case studies in autonomous driving, sign language recognition, music generation, and NLP using TensorFlow and Python."

  - title: "Natural Language Processing Specialization"
    subtitle: "DeepLearning.AI (Coursera)"
    status: "In progress"
    points:
      - "RNNs, LSTMs, GRUs, and Siamese networks in TensorFlow and Trax for sentiment analysis, text generation, and named entity recognition."
      - "Encoder-decoder and self-attention models for machine translation, summarization, chatbots, and question answering."
---

{% include_relative _style.html %}

<div class="ed">

{% assign sections = "education|Education,experience|Work experience,certifications|Certifications" | split: "," %}
{% for sec in sections %}
  {% assign parts = sec | split: "|" %}
  {% assign key = parts[0] %}
  {% assign items = page[key] %}

<h2 class="ed-h">{{ parts[1] }}</h2>

<div class="ed-list">
  {% for it in items %}
  <article class="ed-item">

    <div class="ed-dot"></div>

    <div class="ed-card">

      <div class="ed-top">
        <h3 class="ed-title">
          {% if it.url %}<a href="{{ it.url }}">{{ it.title }}</a>{% else %}{{ it.title }}{% endif %}
        </h3>
        {% if it.period %}<span class="ed-period">{{ it.period }}</span>{% endif %}
        {% if it.status %}<span class="ed-status {% if it.status == 'Completed' %}done{% endif %}">{{ it.status }}</span>{% endif %}
      </div>

      {% if it.subtitle or it.location %}
      <p class="ed-sub">
        {{ it.subtitle }}{% if it.subtitle and it.location %} &middot; {% endif %}<span class="ed-loc">{{ it.location }}</span>
      </p>
      {% endif %}

      {% if it.facts %}
      <div class="ed-facts">
        {% for f in it.facts %}<span class="ed-fact">{{ f }}</span>{% endfor %}
      </div>
      {% endif %}

      {% if it.points %}
      <ul class="ed-points">
        {% for p in it.points %}<li>{{ p }}</li>{% endfor %}
      </ul>
      {% endif %}

    </div>

  </article>
  {% endfor %}
</div>

{% endfor %}

</div>
