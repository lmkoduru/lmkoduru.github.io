---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---


{% include base_path %}

{% for post in site.publications reversed %}
  {% unless post.section == 'posters-workshops' %}
    {% include archive-single.html %}
  {% endunless %}
{% endfor %}

<h1 class="page__title pub-section-title">Posters and Workshops</h1>

{% for post in site.publications reversed %}
  {% if post.section == 'posters-workshops' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
