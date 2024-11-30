---
layout: collection
title: "Hi! I'm Eric Sigg"
collection: portfolio
entries_layout: grid
permalink: /
---


Welcome to my portfolio! I'm excited to show off some of the projects I've worked on throughout my time at the University of Pennsylvania, both in academic courses as well as for my own original research.

PLACEHOLDER IMAGE
![My Image](/assets/images/IMG_5727.JPG)


<div class="portfolio-grid">
  {% for item in site.portfolio %}
    <div class="portfolio-item">
      <a href="{{ item.url | relative_url }}">
        {% if item.image %}
          <img src="{{ item.image | relative_url }}" alt="{{ item.title }}">
        {% endif %}
        <h3>{{ item.title }}</h3>
        <p>{{ item.description }}</p>
      </a>
    </div>
  {% endfor %}
</div>