---
title: "ML/LLM Projects"
permalink: /ml-llm
---

<section>
  <p>Selected LLM + ML work. Each card links to code and/or writeups.</p>
  <div class="cards">
  {% for p in site.data.ml_projects %}
    <article class="card">
      <h3>{{ p.title }}</h3>
      <p>{{ p.summary }}</p>
      {% if p.stack %}<p>{% for s in p.stack %}<span class="pill">{{ s }}</span>{% endfor %}</p>{% endif %}
      <p>
        {% if p.repo %}
          {% if p.repo contains "http" %}
            <a href="{{ p.repo }}" target="_blank" rel="noopener">Repo</a>
          {% else %}
            <a href="{{ p.repo | relative_url }}">Repo</a>
          {% endif %}
        {% endif %}
        {% if p.report %}
          {% if p.report contains "http" %}
            · <a href="{{ p.report }}" target="_blank" rel="noopener">Report</a>
          {% else %}
            · <a href="{{ p.report | relative_url }}">Report</a>
          {% endif %}
        {% endif %}
        {% if p.demo %}
          {% if p.demo contains "http" %}
            · <a href="{{ p.demo }}" target="_blank" rel="noopener">Demo</a>
          {% else %}
            · <a href="{{ p.demo | relative_url }}">Demo</a>
          {% endif %}
        {% endif %}
      </p>
    </article>
  {% endfor %}
  </div>
</section>
