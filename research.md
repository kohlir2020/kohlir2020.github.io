---
title: "Research Projects"
permalink: /research
---

<section>
  <p>Selected research. Links to papers, preprints, and extended summaries as available.</p>
  <div class="cards">
  {% for p in site.data.research_projects %}
    <article class="card">
      <h3>{{ p.title }}</h3>
      <p>{{ p.summary }}</p>
      {% if p.stack %}<p>{% for s in p.stack %}<span class="pill">{{ s }}</span>{% endfor %}</p>{% endif %}
      <p>
        {% if p.link %}
          {% if p.link contains "http" %}
            <a href="{{ p.link }}" target="_blank" rel="noopener">Link</a>
          {% else %}
            <a href="{{ p.link | relative_url }}">Link</a>
          {% endif %}
        {% endif %}
        {% if p.preprint %}
          {% if p.preprint contains "http" %}
            · <a href="{{ p.preprint }}" target="_blank" rel="noopener">Preprint</a>
          {% else %}
            · <a href="{{ p.preprint | relative_url }}">Preprint</a>
          {% endif %}
        {% endif %}
        {% if p.extended %}
          {% if p.extended contains "http" %}
            · <a href="{{ p.extended }}" target="_blank" rel="noopener">Extended summary</a>
          {% else %}
            · <a href="{{ p.extended | relative_url }}">Extended summary</a>
          {% endif %}
        {% endif %}
      </p>
    </article>
  {% endfor %}
  </div>
</section>
