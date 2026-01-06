---
title: "Augmenting biomedical named entity recognition with general-domain resources"
collection: publications
permalink: /publication/2024-10-04-bioner-gerbera
date: 2024-10-04
venue: 'Journal of Biomedical Informatics'
paperurl: 'https://doi.org/10.1016/j.jbi.2024.104731'
citation: 'Yu Yin* and Hyunjae Kim* and Xiao Xiao and Chih Hsuan Wei and Jaewoo Kang and Zhiyong Lu and Hua Xu and Meng Fang and Qingyu Chen.'
abstract: 'Biomedical NER requires specialized domain knowledge. We propose leveraging general-domain resources to augment biomedical NER models, improving performance on limited labeled data.'
tags: ['Biomedical NLP']
image: '/images/gerbera_abstract.jpg'
---

<div class="publication-container">
  <div class="publication-image">
    <img src="{{ page.image }}" alt="Paper illustration">
  </div>
  
  <div class="publication-content">
    <h3 class="publication-title">{{ page.title }}</h3>
    
    <p class="publication-meta">
      <span class="publication-venue">{{ page.venue }}</span>
      <span class="publication-year">{{ page.date | date: "%Y" }}</span>
    </p>
    
    <div class="publication-tags">
      {% for tag in page.tags %}
        <span class="tag">{{ tag }}</span>
      {% endfor %}
    </div>
    
    <p class="publication-abstract">
      <strong>Abstract:</strong> {{ page.abstract }}
    </p>
    
    <div class="publication-links">
      <a href="{{ page.paperurl }}" class="publication-link">
        <i class="fas fa-file-pdf"></i> Paper
      </a>
      <a href="#" class="publication-link">
        <i class="fas fa-code"></i> Code
      </a>
      <a href="#" class="publication-link">
        <i class="fas fa-link"></i> Project
      </a>
    </div>
  </div>
</div>
