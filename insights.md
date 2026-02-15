---
title: Insights
permalink: /insights/
layout: default
---

<section class="section">
  <div class="section-title">
    <h2>Insights</h2>
    <div class="hint">Operator-grade thinking.</div>
  </div>

  <div class="grid">
    {% for post in site.posts %}
      <a class="card" href="{{ post.url | relative_url }}" style="grid-column: span 12;">
        <h3 style="margin-bottom:6px;">{{ post.title }}</h3>
        <p style="margin:0 0 8px;" class="small">{{ post.date | date: "%b %d, %Y" }}</p>
        <p style="margin:0;">{{ post.excerpt | strip_html | truncate: 160 }}</p>
      </a>
    {% endfor %}
  </div>
</section>
