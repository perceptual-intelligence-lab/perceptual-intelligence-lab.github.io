---
title: "News"
layout: splash
permalink: /news/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/news-hero-image.jpg
  actions:
    - label: "Subscribe"
      url: "#"
      class: "btn--primary"
  caption: "Stay up to date with the latest news from our lab"
excerpt: "Recent updates, publications, and announcements from the Perceptual Intelligence Lab."
intro:
  - excerpt: 'Find all the latest updates and announcements here.'
---

{% include feature_row id="intro" type="center" %}

<div class="news-grid">
  {% for post in site.categories.news limit:3 %}
  <div class="news-item">
    <a href="{{ post.url }}">
      <div class="news-thumb" style="background-image: url('{{ post.image }}');"></div>
      <div class="news-content">
        <h3>{{ post.title }}</h3>
        <p>{{ post.excerpt }}</p>
        <a href="{{ post.url }}" class="btn btn--primary">Read More</a>
      </div>
    </a>
  </div>
  {% endfor %}
</div>
