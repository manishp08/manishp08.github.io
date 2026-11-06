---
layout: default
---

## About
A short intro about you.

## Projects

<div class="projects">
{% for p in site.data.projects %}
  <div class="project">
    <h3><a href="{{ p.repo }}">{{ p.title }}</a></h3>
    <p class="project-url">{{ p.repo | remove: "https://" }}</p>
    <p>{{ p.description }}</p>
    <p class="tags">
      {% for t in p.tech %}<span>{{ t }}</span>{% endfor %}
    </p>
    <p class="links">
      <a href="{{ p.repo }}">GitHub</a>
      {% if p.demo %} · <a href="{{ p.demo }}">Demo</a>{% endif %}
    </p>
  </div>
{% endfor %}
</div>

## Contact
pmanishkumarcareers@gmail.com