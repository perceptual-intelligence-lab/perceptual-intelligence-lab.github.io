---
title: "Team"
layout: default
permalink: /people/
---

# Meet The Team

## Director
<div class="team-row">
  {% for person in site.people %}
    {% if person.jobtitle == "Director" %}
      <div class="team-member">
        <img src="{{ person.image }}" alt="{{ person.title }}">
        <h2>{{ person.title }}</h2>
        <p>{{ person.content | markdownify }}</p>
      </div>
    {% endif %}
  {% endfor %}
</div>

## Junior PIs
<div class="team-row">
  {% for person in site.people %}
    {% if person.jobtitle == "Junior PI" %}
      <div class="team-member">
        <img src="{{ person.image }}" alt="{{ person.title }}">
        <h2>{{ person.title }}</h2>
        <p>{{ person.content | markdownify }}</p>
      </div>
    {% endif %}
  {% endfor %}
</div>

## Students
<div class="team-row">
  {% for person in site.people %}
    {% if person.jobtitle == "Student" %}
      <div class="team-member">
        <img src="{{ person.image }}" alt="{{ person.title }}">
        <h2>{{ person.title }}</h2>
        <p>{{ person.content | markdownify }}</p>
      </div>
    {% endif %}
  {% endfor %}
</div>

## Research Assistants
<div class="team-row">
  {% for person in site.people %}
    {% if person.jobtitle == "Research Assistant" %}
      <div class="team-member">
        <img src="{{ person.image }}" alt="{{ person.title }}">
        <h2>{{ person.title }}</h2>
        <p>{{ person.content | markdownify }}</p>
      </div>
    {% endif %}
  {% endfor %}
</div>
