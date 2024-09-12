---
title: Meet The Team
layout: default
permalink: /team/
---

# Meet The Team

## Director
<div class="team-grid">
    {% assign directors = site.team | where: "role", "director" %}
    {% for person in directors %}
    <div class="team-member">
        <img src="{{ person.image }}" alt="{{ person.title }}" />
        <h3>{{ person.title }}</h3>
        <p>{{ person.excerpt }}</p>
    </div>
    {% endfor %}
</div>

## Junior PIs
<div class="team-grid">
    {% assign junior_pis = site.team | where: "role", "junior pi" %}
    {% for person in junior_pis %}
    <div class="team-member">
        <img src="{{ person.image }}" alt="{{ person.title }}" />
        <h3>{{ person.title }}</h3>
        <p>{{ person.excerpt }}</p>
    </div>
    {% endfor %}
</div>

## Students
<div class="team-grid">
    {% assign students = site.team | where: "role", "student" %}
    {% for person in students %}
    <div class="team-member">
        <img src="{{ person.image }}" alt="{{ person.title }}" />
        <h3>{{ person.title }}</h3>
        <p>{{ person.excerpt }}</p>
    </div>
    {% endfor %}
</div>

## Research Assistants
<div class="team-grid">
    {% assign assistants = site.team | where: "role", "research assistant" %}
    {% for person in assistants %}
    <div class="team-member">
        <img src="{{ person.image }}" alt="{{ person.title }}" />
        <h3>{{ person.title }}</h3>
        <p>{{ person.excerpt }}</p>
    </div>
    {% endfor %}
</div>
