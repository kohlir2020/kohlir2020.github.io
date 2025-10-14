---
title: "Extracurricular"
permalink: /extracurricular
---

<section>
  <p>Teaching, leadership, and volunteer work.</p>
  <div class="cards">
  {% for x in site.data.extracurricular %}
    <article class="card">
      <h3>{{ x.title }}</h3>
      <p>{{ x.summary }}</p>
      {% if x.links %}
        <p>{% for L in x.links %}
          {% if L.url contains "http" %}
            <a href="{{ L.url }}" target="_blank" rel="noopener">{{ L.text }}</a>
          {% else %}
            <a href="{{ L.url | relative_url }}">{{ L.text }}</a>
          {% endif %}
          {% unless forloop.last %} · {% endunless %}
        {% endfor %}</p>
      {% endif %}
    </article>
  {% endfor %}
  </div>
</section>