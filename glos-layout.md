---
description: Sample layout
---

# Glos Layout

General introductory text

## Term 1a

term1 definition

## Term 2

Term2 def

# Try rendering collections
{% for term in site.glosssary %}
  <h2>{{ term.name }} - {{ term.position }}</h2>
  <p>{{ term.content | markdownify }}</p>
{% endfor %}
