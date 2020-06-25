---
layout: glossary
---
# glos-layout2.md using glossary layout in front matter
# Try rendering glossary collection
{% for term in site.glossary %}
  # {{ term.name }}
  Source: {{ term.page.name }}, path: {{ term.path }}
  [Page link]({{ term.url }})
  Content:
  {{ term.content }}
  ---
{% endfor %}

## end render

This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.
