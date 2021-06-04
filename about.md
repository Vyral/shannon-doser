---
layout: about
title: About
permalink: /about/
---

&nbsp;
{% for item in site.data.agents.agent %}
  <div class="recruiting-photo"><span class="client-image-container"><img alt="{{item.name}}" class="client-image" src="{{item.photo}}" /> </span></div>

  <h3>{{item.name}}</h3>

  <p class="testimonial">{{item.bio | markdownify }}</p>

  <hr>
{% endfor %}
