---
layout: default
title: "Meet the Team"
permalink: /people/
---

# Meet the Team

Our team of researchers and scientists are dedicated to advancing the field of perceptual intelligence.

## Director
<div class="team-section">
{% for person in site.people %}
    {% if person.role == "director" %}
    <div class="team-member">
        <img src="{{ person.image }}" alt="{{ person.name }}" class="team-image"/>
        <h3>{{ person.name }}</h3>
    </div>
    {% endif %}
{% endfor %}
</div>

## Junior PI
<div class="team-section">
{% for person in site.people %}
    {% if person.role == "junior pi" %}
    <div class="team-member">
        <img src="{{ person.image }}" alt="{{ person.name }}" class="team-image"/>
        <h3>{{ person.name }}</h3>
    </div>
    {% endif %}
{% endfor %}
</div>

## Students
<div class="team-section">
{% for person in site.people %}
    {% if person.role == "student" %}
    <div class="team-member">
        <img src="{{ person.image }}" alt="{{ person.name }}" class="team-image"/>
        <h3>{{ person.name }}</h3>
    </div>
    {% endif %}
{% endfor %}
</div>

## Research Assistants
<div class="team-section">
{% for person in site.people %}
    {% if person.role == "research assistant" %}
    <div class="team-member">
        <img src="{{ person.image }}" alt="{{ person.name }}" class="team-image"/>
        <h3>{{ person.name }}</h3>
    </div>
    {% endif %}
{% endfor %}
</div>

<style>
.team-section {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    margin-bottom: 40px;
}

.team-member {
    flex: 1 1 30%;
    text-align: center;
    border: 1px solid #f0f0f0;
    padding: 20px;
    background-color: #f9f9f9;
}

.team-image {
    width: 150px;
    height: auto;
    margin-bottom: 15px;
    object-fit: cover;
}

h3 {
    margin-top: 10px;
    font-size: 1.5em;
}

h2, h3 {
    font-family: Arial, sans-serif;
    color: #333;
}

p {
    font-size: 1em;
    margin-bottom: 10px;
}
</style>
