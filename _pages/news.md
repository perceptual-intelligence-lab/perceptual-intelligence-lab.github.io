---
layout: default
title: News
permalink: /news/
---

<!-- Featured News Section -->
<section class="featured-posts">
    <div class="section-title">
        <h2><span>Featured News</span></h2>
    </div>
    <div class="row">

    {% for post in site.posts %}
        {% if post.featured == true and post.categories contains 'news' %}
            {% include featuredbox.html %}
        {% endif %}
    {% endfor %}

    </div>
</section>

<!-- All News Section -->
<section class="recent-posts">
    <div class="section-title">
        <h2><span>All News</span></h2>
    </div>

    <div class="row listrecent">
        {% for post in paginator.posts %}
            {% if post.categories contains 'news' %}
                {% include postbox.html %}
            {% endif %}
        {% endfor %}
    </div>
</section>

<!-- Pagination for News -->
<div class="bottompagination">
    <div class="pointerup"><i class="fa fa-caret-up"></i></div>
    <span class="navigation" role="navigation">
        {% include pagination.html %}
    </span>
</div>
