---
layout: default
title: "Home"
description: "Machine Learning Software Engineer and Researcher specializing in Reinforcement Learning, Computer Vision, and AI applications. Explore my projects, publications, and research work."
image: /assets/img/site-image.jpg
---

<div class="hero">
  <h1>Raunit Kohli</h1>
  <p class="hero-tagline">Machine Learning Engineer building autonomous systems that bridge AI research and real-world applications.</p>
  <p class="hero-description">I develop reinforcement learning algorithms and computer vision systems that solve complex problems—from autonomous robot-animal interactions processing 2500+ experiments to enterprise API testing frameworks with 780+ automated tests. My work spans cutting-edge research and production-ready software engineering.</p>
  
  <div class="hero-links">
    <a href="{{ '/projects/' | relative_url }}" class="hero-link">View Projects</a>
    <a href="{{ '/publications/' | relative_url }}" class="hero-link">Research</a>
    <a href="{{ '/assets/Raunit_Resume_Aug_25.pdf' | relative_url }}" class="hero-link" target="_blank" rel="noopener">Download CV</a>
  </div>
</div>

## Featured Projects

{% assign featured_projects = site.projects | where: 'featured', true | sort: 'year' | reverse %}
{% if featured_projects.size > 0 %}
<div class="featured-projects-grid">
  {% for project in featured_projects %}
  <div class="featured-project-card">
    <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
    <p class="project-meta">{{ project.year }} • {{ project.role }}</p>
    <p class="project-summary">{{ project.summary }}</p>
    <div class="project-highlights">
      {% for highlight in project.highlights limit:2 %}
        <p class="highlight-item">• {{ highlight }}</p>
      {% endfor %}
    </div>
    <div class="project-tech">
      {% for tech in project.tech limit:5 %}
        <span class="tech-pill">{{ tech }}</span>
      {% endfor %}
    </div>
    <a href="{{ project.url | relative_url }}" class="project-cta">Learn More →</a>
  </div>
  {% endfor %}
</div>
{% endif %}

## Featured Publications

{% assign featured_publications = site.publications | where: 'featured', true | sort: 'year' | reverse %}
{% if featured_publications.size > 0 %}
<div class="featured-publications-grid">
  {% for pub in featured_publications %}
  <div class="featured-publication-card">
    <h3><a href="{{ pub.url }}">{{ pub.title }}</a></h3>
    <p class="publication-meta">
      {% for author in pub.authors %}
        {% if author == "Raunit Kohli" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% unless forloop.last %}, {% endunless %}
      {% endfor %}
    </p>
    <p class="publication-venue">{{ pub.venue }}, {{ pub.year }}</p>
    <p class="publication-abstract">{{ pub.abstract | truncate: 200 }}</p>
    <div class="publication-links">
      {% if pub.url and pub.url != "" %}
        <a href="{{ pub.url }}" target="_blank" rel="noopener" class="pub-link">Read Paper</a>
      {% endif %}
      {% if pub.doi and pub.doi != "" %}
        <a href="https://doi.org/{{ pub.doi }}" target="_blank" rel="noopener" class="pub-link">DOI</a>
      {% endif %}
      <a href="{{ pub.url }}" class="pub-link">Details</a>
    </div>
  </div>
  {% endfor %}
</div>
{% endif %}

## Let's Connect

<div class="cta-strip">
  <div class="cta-content">
    <h3>Ready to collaborate on the next breakthrough?</h3>
    <p>Whether you're interested in machine learning research, autonomous systems, or building scalable software—let's talk.</p>
  </div>
  <div class="cta-buttons">
    <a href="https://github.com/kohlir2020" target="_blank" rel="noopener" class="cta-btn cta-github">
      <span class="btn-icon">📁</span>
      GitHub
    </a>
    <a href="https://linkedin.com/in/raunit-kohli-34b944157" target="_blank" rel="noopener" class="cta-btn cta-linkedin">
      <span class="btn-icon">💼</span>
      LinkedIn
    </a>
    <a href="mailto:raunit.kohli@gmail.com" class="cta-btn cta-email">
      <span class="btn-icon">✉️</span>
      Email
    </a>
  </div>
</div>