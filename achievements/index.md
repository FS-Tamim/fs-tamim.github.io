---
title: "Achievements & Skills"
excerpt: ""
author_profile: true
permalink: /achievements/

# ==============================================================
#  ACHIEVEMENTS & SKILLS PAGE  -  everything lives in /achievements
#
#    achievements/index.md    <- this file: all the content
#    achievements/_style.html <- colors and spacing
#
#  To add an entry, copy one block (from "- title:" to its last
#  line), paste it at the TOP of the right section, and edit it.
#  Keep the same indentation. Delete any line you don't need.
#
#  HONORS FIELDS
#    rank  : short badge, e.g. "2nd Runner-up", "14th Place"
#    title : competition / task name
#    event : where it was held
#    date  : e.g. "May 2023"
#    url   : link (optional)
#
#  ACTIVITY FIELDS
#    org, role, period, place
#
#  SKILL FIELDS
#    group : category name
#    items : list of skills
# ==============================================================


# ---------------- HONORS AND AWARDS ----------------
honors:

  - rank: "14th Place"
    title: "Detecting Signs of Depression from Social Media Text"
    event: "LT-EDI 2023 Shared Task @ RANLP 2023"
    date: "May 2023"

  - rank: "2nd Runner-up"
    title: "Multimodal Sentiment Analysis"
    event: "Computational Linguistics and Bangla Language Processing (CLBLP 2023)"
    date: "Feb 2023"

  - rank: "2nd Runner-up"
    title: "Sentiment Analysis of Code-Mixed Text"
    event: "Computational Linguistics and Bangla Language Processing (CLBLP 2023)"
    date: "Feb 2023"

  - rank: "Onsite Participant"
    title: "Natural Language Processing Hackathon"
    event: "Bangladesh Open Source Network (BdOSN)"
    date: "Oct 2022"

  - rank: "Participant"
    title: "Datathon 2.0"
    event: "Robi Axiata Limited"
    date: "Sep 2021"


# ---------------- SERVICE AND LEADERSHIP ----------------
activities:

  - org: "Workshop on Detecting AI Generated Content @ COLING 2025"
    role: "Program Committee Member"
    period: "2025"
    place: "Abu Dhabi, UAE"

  - org: "CUET Computer Club"
    role: "General Secretary"
    period: "2022 - 2023"
    place: "CUET"

  - org: "Remians' Association of CUET"
    role: "General Secretary"
    period: "2022 - 2023"
    place: "CUET"

  - org: "Notredamian Association of CUET"
    role: "Joint General Secretary"
    period: "2022 - 2023"
    place: "CUET"

  - org: "Green for Peace"
    role: "Archive Secretary"
    period: "2022 - 2023"
    place: "CUET"

  - org: "CUET CSE Fest 2022"
    role: "Organizing Secretary"
    period: "2022"
    place: "Department of CSE, CUET"

  - org: "Department of CSE, CUET"
    role: "Class Representative"
    period: "2019 - 2023"
    place: "CUET"


# ---------------- TECHNICAL SKILLS ----------------
skills:

  - group: "Programming languages"
    proficient: ["Python", "C", "C++"]
    familiar: ["Java", "JavaScript", "SQL"]

  - group: "Machine learning and deep learning"
    proficient: ["PyTorch", "TensorFlow", "Keras", "Scikit-learn"]

  - group: "NLP and data"
    proficient: ["NLTK", "Gensim", "Pandas", "OpenCV"]

  - group: "Web development"
    familiar: ["MERN stack", "MySQL"]

  - group: "Tools"
    proficient: ["Git", "Jupyter", "LaTeX"]
---

{% include_relative _style.html %}

<div class="ac">


<!-- ================= Honors and awards ================= -->

<h2 class="ac-h">Honors and awards</h2>

<div class="ac-honors">
  {% for h in page.honors %}
  <article class="honor">
    <span class="honor-rank {% if h.rank contains 'Participant' %}plain{% endif %}">{{ h.rank }}</span>
    <div class="honor-body">
      <h3 class="honor-title">{% if h.url %}<a href="{{ h.url }}">{{ h.title }}</a>{% else %}{{ h.title }}{% endif %}</h3>
      <p class="honor-event">{{ h.event }}</p>
    </div>
    <span class="honor-date">{{ h.date }}</span>
  </article>
  {% endfor %}
</div>


<!-- ================= Service and leadership ================= -->

<h2 class="ac-h">Service and leadership</h2>

<div class="ac-grid">
  {% for a in page.activities %}
  <article class="act">
    <p class="act-role">{{ a.role }}</p>
    <h3 class="act-org">{{ a.org }}</h3>
    <p class="act-meta">{{ a.period }} &middot; {{ a.place }}</p>
  </article>
  {% endfor %}
</div>


<!-- ================= Technical skills ================= -->

<h2 class="ac-h">Technical skills</h2>

<div class="ac-skills">
  {% for s in page.skills %}
  <div class="skill-row">
    <span class="skill-group">{{ s.group }}</span>
    <span class="skill-items">
      {% for i in s.proficient %}<span class="chip">{{ i }}</span>{% endfor %}
      {% for i in s.familiar %}<span class="chip chip-light">{{ i }}</span>{% endfor %}
    </span>
  </div>
  {% endfor %}
</div>

<p class="ac-legend">
  <span class="chip">Proficient</span>
  <span class="chip chip-light">Familiar</span>
</p>


</div>
