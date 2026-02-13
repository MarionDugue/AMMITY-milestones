---
layout: default
title: Learning about menstruation
---

# Educational Resources
Welcome to our learning hub. Here you will find detailed information regarding menstruation health and research.

---

<div class="article-list">
  {% for article in site.articles %}
    <div class="article-card" onclick="location.href='{{ article.url | relative_url }}'">
      <h2>{{ article.title }}</h2>
      <p>{{ article.excerpt | strip_html | truncate: 160 }}</p>
      <span class="read-more-link">Read full article →</span>
    </div>
  {% endfor %}
</div>

<style>
  .article-card {
    background: var(--white);
    padding: 2rem;
    margin-bottom: 2rem;
    border-radius: 20px;
    cursor: pointer;
    transition: 0.3s;
    border: 2px solid transparent;
  }
  .article-card:hover {
    border-color: var(--accent);
    transform: translateY(-5px);
  }
  .read-more-link {
    color: var(--accent);
    font-weight: bold;
  }
</style>
