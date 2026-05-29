---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a first-year PhD student at the University of Queensland, working under the guidance of [Prof. Guido Zuccon](https://about.uq.edu.au/experts/22857), [Assoc. Prof. Bevan Koopman](https://bevankoopman.github.io/), and [Dr. Shuai Wang](https://wshuai190.github.io/). My research sits at the intersection of information retrieval, large language models, and biomedical applications.

## **Recent News**

<ol class="news-list">
{% assign news = site.data.news | sort: 'date' | reverse %}
{% for item in news %}
  <li class="news-item">
    <span class="news-date">[{{ item.date | date: "%Y.%m.%d" }}]</span> {{ item.content }}
  </li>
{% endfor %}
</ol>

## **Education**
- PhD in Computer Science, University of Queensland (2026–present)
- Master's in Computer Science, Imperial College London (2023–2024), supervised by [Dr. Qingyu Chen](https://medicine.yale.edu/profile/qingyu-chen/)
- Bachelor's in Computer Science, Xi'an Jiaotong-Liverpool University and University of Liverpool (2019–2023), supervised by [Dr. Meng Fang](https://mengfn.github.io/)

## **Work Experience**
- Research Assistant, School of Biomedical Informatics and Data Science, Yale University (2024–2025), supervised by [Dr. Qingyu Chen](https://medicine.yale.edu/profile/qingyu-chen/)

## **Academic Services**
- Conference reviewer — ACL
- Journal reviewer — ACM Trans. on Computing for Healthcare
- Volunteer, EMNLP 2025, Suzhou

## **Research Interests**

My research focuses on information retrieval, multimodal analysis of large language models, and artificial intelligence-assisted biomedical applications.
