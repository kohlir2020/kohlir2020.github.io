---
layout: default
title: "Publications"
description: "Academic publications and research contributions by Raunit Kohli in machine learning, cognitive science, robotics, and artificial intelligence."
---

# Publications

<p class="page-intro">Academic publications and research contributions.</p>

{% assign sorted_publications = site.publications | sort: 'date' | reverse %}
{% if sorted_publications.size > 0 %}
  <div class="publications-list">
    {% for publication in sorted_publications %}
      {% include publication_item.html publication=publication %}
    {% endfor %}
  </div>
{% else %}
  <div class="empty-state">
    <p>No publications have been added yet. Check back soon!</p>
  </div>
{% endif %}