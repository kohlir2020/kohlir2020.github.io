---
layout: default
title: "Projects"
description: "Explore Raunit Kohli's portfolio of machine learning projects including robotics, reinforcement learning, computer vision, and AI applications in research and industry."
---

# Projects

<p class="page-intro">A collection of projects spanning research, development, and innovation.</p>

{% assign sorted_projects = site.projects | sort: 'date' | reverse %}
{% if sorted_projects.size > 0 %}
  <div class="projects-list">
    {% for project in sorted_projects %}
      {% include project_item.html project=project %}
    {% endfor %}
  </div>
{% else %}
  <div class="empty-state">
    <p>No projects have been added yet. Check back soon!</p>
  </div>
{% endif %}