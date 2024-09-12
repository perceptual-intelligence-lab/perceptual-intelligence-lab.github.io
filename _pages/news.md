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
feature_row2:
  - image_path: /assets/images/news-image-1.jpg
    alt: "News Image 1"
    title: "New Publication on Perception"
    excerpt: "We recently published a groundbreaking study on how the brain processes visual information..."
    url: "/news/publication-perception"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row3:
  - image_path: /assets/images/news-image-2.jpg
    alt: "News Image 2"
    title: "Join Our Open Day Event"
    excerpt: "Come visit our lab and see the work we're doing in perceptual intelligence..."
    url: "/news/open-day-event"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row4:
  - image_path: /assets/images/news-image-3.jpg
    alt: "News Image 3"
    title: "Conference Presentation at Neuroscience 2024"
    excerpt: "Our lab will be presenting at the upcoming neuroscience conference..."
    url: "/news/conference-neuroscience-2024"
    btn_label: "Read More"
    btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}

<div class="news-grid">
  {% include feature_row id="feature_row2" type="left" %}
  {% include feature_row id="feature_row3" type="right" %}
  {% include feature_row id="feature_row4" type="left" %}
</div>
