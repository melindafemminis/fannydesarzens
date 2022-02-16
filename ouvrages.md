---
layout: page
title: Ouvrages
permalink: /ouvrages/
---

<!-- {% for ouvrage in site.ouvrages %}
  <img src="{{ ouvrage.img}}" height="500px"><br>
  **{{ ouvrage.title }}**, {{ ouvrage.year }} | {{ ouvrage.editions }} - {{ ouvrage.type }}
{% endfor %} -->

<div class="main">
  <ul class="cards">
{% for ouvrage in site.ouvrages %}
      <li class="cards_item">
        <div class="card">
          <div class="img"><img src="{{ ouvrage.img}}"></div>
          <div class="card_content">
            <h2 class="card_title">{{ ouvrage.titre }}</h2>
            <p class="card_text">{{ ouvrage.year }} | {{ ouvrage.editions }} - {{ ouvrage.type }}</p>
            <button class="btn card_btn">Lis-moi</button>
          </div>
        </div>
      </li>
{% endfor %}
  </ul>
</div>
