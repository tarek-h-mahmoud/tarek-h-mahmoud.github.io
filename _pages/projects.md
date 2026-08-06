---
layout: page
title: Selected Projects
permalink: /projects/
nav: true
nav_order: 3
description: Production AI systems and applied research across government, finance, and public health.
_styles: |
  .proj-group {
    margin-top: 3rem;
  }

  .proj-group:first-of-type {
    margin-top: 1.5rem;
  }

  .proj-group-title {
    font-size: 1rem;
    font-weight: 700;
    letter-spacing: 0.07em;
    text-transform: uppercase;
    color: var(--global-text-color);
    padding-bottom: 0.55rem;
    border-bottom: 2px solid var(--global-theme-color);
    margin-bottom: 1.75rem;
  }

  /* The whole card is a single <a>, so the entire rectangle is
     clickable and gets one entry in the tab order rather than two. */
  .proj-card {
    display: block;
    color: inherit;
    text-decoration: none;
    padding: 1.1rem 1rem;
    margin: 0 -1rem;
    border-radius: 6px;
    border-bottom: 1px solid var(--global-divider-color);
    transition: background-color 0.15s ease;
  }

  .proj-card:hover {
    background-color: var(--global-code-bg-color);
    text-decoration: none;
  }

  .proj-card:focus-visible {
    outline: 2px solid var(--global-theme-color);
    outline-offset: 2px;
  }

  .proj-card:last-child {
    border-bottom: none;
  }

  .proj-card-title {
    font-size: 1.15rem;
    font-weight: 600;
    margin: 0;
    line-height: 1.35;
    color: var(--global-theme-color);
  }

  .proj-card:hover .proj-card-title {
    text-decoration: underline;
  }

  .proj-context {
    font-size: 0.85rem;
    color: var(--global-text-color-light);
    margin-top: 0.15rem;
  }

  .proj-summary {
    margin-top: 0.6rem;
    line-height: 1.6;
  }

  .proj-tech {
    margin-top: 0.75rem;
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
  }

  .proj-tech span {
    font-size: 0.7rem;
    letter-spacing: 0.02em;
    padding: 0.15rem 0.5rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 3px;
    color: var(--global-text-color-light);
    white-space: nowrap;
  }

---

{% assign ordered = site.projects | sort: "order" %}
{% assign group_names = "Product Development,Large-Scale Decision Systems,Applied ML & Data Systems" | split: "," %}

{% for group_name in group_names %}
  <section class="proj-group">
    <h2 class="proj-group-title">{{ group_name }}</h2>
    {% for project in ordered %}
      {% if project.group == group_name %}
        <a class="proj-card" href="{{ project.permalink | relative_url }}">
          <h3 class="proj-card-title">{{ project.title }}</h3>
          {% if project.context %}<div class="proj-context">{{ project.context }}</div>{% endif %}
          <div class="proj-summary">{{ project.summary }}</div>
          {% if project.tech %}
            <div class="proj-tech">
              {% for t in project.tech %}<span>{{ t }}</span>{% endfor %}
            </div>
          {% endif %}
        </a>
      {% endif %}
    {% endfor %}
  </section>
{% endfor %}
