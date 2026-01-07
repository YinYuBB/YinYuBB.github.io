---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<div class="publications-list">
  {% for post in site.publications reversed %}
    <div class="publication-container">
      
      <div class="publication-image">
        {% if post.image %}
          <img src="{{ post.image | prepend: base_path }}" alt="{{ post.title }}">
        {% else %}
          <div style="color:#ddd; font-size:0.8rem;"></div>
        {% endif %}
      </div>
      
      <div class="publication-content">
        <h3 class="publication-title">{{ post.title }}</h3>
        
        {% if post.citation %}
          <div class="publication-authors">
            {{ post.citation | replace: 'Yu Yin', '<b>Yu Yin</b>' | replace: 'Yin, Yu', '<b>Yin, Yu</b>' }}
          </div>
        {% endif %}
        
        <p class="publication-meta">
          <span class="publication-venue">{{ post.venue }}</span>
          <span class="publication-year">{{ post.date | date: "%Y" }}</span>
        </p>
        
        {% if post.tags %}
          <div class="publication-tags">
            {% for tag in post.tags %}
              <span class="tag">{{ tag }}</span>
            {% endfor %}
          </div>
        {% endif %}
        
        {% if post.abstract %}
          <div class="publication-abstract">
            <strong>Abstract:</strong> {{ post.abstract }}
          </div>
        {% endif %}
        
        <div class="publication-links">
          {% if post.paperurl %}
            <a href="{{ post.paperurl }}" class="publication-link" target="_blank">📄 Paper</a>
          {% endif %}
          
          {% if post.codeurl %}
            <a href="{{ post.codeurl }}" class="publication-link" target="_blank">💻 Code</a>
          {% endif %}
          
          {% if post.projecturl %}
            <a href="{{ post.projecturl }}" class="publication-link" target="_blank">🔗 Project</a>
          {% endif %}
        </div>
      </div>
    </div>
  {% endfor %}
</div>