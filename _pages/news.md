---
title: "News"
layout: splash
permalink: /news/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/news.jpg
  caption: "Stay up to date with the latest news from our lab."
excerpt: "Recent updates, publications, and announcements from the Perceptual Intelligence Lab."
---

{% include feature_row id="intro" type="center" %}

<!-- Dynamic Feature Row Loop -->
{% assign posts = site.categories.news limit:3 %}
{% assign feature_row = "" %}

{% for post in posts %}
  {% assign feature_row = feature_row | append: "- image_path: " | append: post.image | append: " \n" %}
  {% assign feature_row = feature_row | append: "  title: " | append: post.title | append: " \n" %}
  {% assign feature_row = feature_row | append: "  excerpt: " | append: post.excerpt | append: " \n" %}
  {% assign feature_row = feature_row | append: "  url: " | append: post.url | append: " \n" %}
  {% if forloop.index < posts.size %}
    {% assign feature_row = feature_row | append: "\n" %}
  {% endif %}
{% endfor %}

{% capture feature_row_content %}
{{ feature_row }}
{% endcapture %}

{% include feature_row %}
