---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<style>
.publication-container {
  display: flex;
  gap: 2rem;
  margin: 2rem 0;
  padding: 1.5rem;
  border: 1px solid rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  background: #ffffff;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.08);
  transition: box-shadow 0.3s ease;
}

.publication-container:hover {
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.12);
}

.publication-image {
  flex-shrink: 0;
  width: 280px;
  height: 200px;
  border-radius: 6px;
  overflow: hidden;
  background: #f5f5f5;
}

.publication-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 6px;
}

.publication-content {
  flex: 1;
  display: flex;
  flex-direction: column;
}

.publication-title {
  font-size: 1rem !important; 
  
  font-weight: 700;
  margin: 0 0 0.4rem;
  line-height: 1.35;
  color: #1a5490;
}

.publication-meta {
  font-size: 0.85em;
  color: #666;
  margin: 0 0 0.8rem;
  font-style: italic;
}

.publication-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 0.4rem;
  margin-bottom: 0.8rem;
}

.tag {
  display: inline-block;
  padding: 0.25rem 0.7rem;
  background: #e8f0f8;
  color: #1a5490;
  border-radius: 16px;
  font-size: 0.75em;
  font-weight: 500;
}

.publication-abstract {
  margin: 0 0 1rem;
  line-height: 1.5;
  color: #333;
  font-size: 0.8em !important;
}

.publication-links {
  display: flex;
  flex-wrap: wrap;
  gap: 1.5rem;
  margin-top: auto;
  padding-top: 0.8rem;
  border-top: 1px solid rgba(0, 0, 0, 0.08);
}

.publication-link {
  display: inline-flex;
  align-items: center;
  gap: 0.4rem;
  text-decoration: none;
  color: #0066cc;
  font-weight: 500;
  font-size: 0.9em;
}

.publication-link:hover {
  text-decoration: underline;
  color: #0052a3;
}

@media (max-width: 768px) {
  .publication-container {
    flex-direction: column;
    gap: 1rem;
  }
  
  .publication-image {
    width: 100%;
    height: auto;
  }
}
</style>

{% include base_path %}

<!-- Display publications as cards directly on this page -->
<div class="publications-list">
  {% for post in site.publications reversed %}
    <div class="publication-container">
      <div class="publication-image">
        {% if post.image %}
          <img src="{{ post.image | prepend: base_path }}" alt="{{ post.title }}">
        {% else %}
          <div style="background: #f0f0f0; padding: 2rem; text-align: center; color: #999;">No Image</div>
        {% endif %}
      </div>
      
      <div class="publication-content">
        <h3 class="publication-title">{{ post.title }}</h3>
        
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
          <p class="publication-abstract">
            <strong>Abstract:</strong> {{ post.abstract }}
          </p>
        {% endif %}
        
        <div class="publication-links">
          {% if post.paperurl %}
            <a href="{{ post.paperurl }}" class="publication-link" target="_blank">
              📄 Paper
            </a>
          {% endif %}
          
          {% if post.codeurl %}
            <a href="{{ post.codeurl }}" class="publication-link" target="_blank">
              💻 Code
            </a>
          {% endif %}
          
          <a href="#" class="publication-link">
            🔗 Project
          </a>
        </div>
      </div>
    </div>
  {% endfor %}
</div>
