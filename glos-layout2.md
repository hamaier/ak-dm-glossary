---
layout: glossary
---
# Try rendering glossary collection
{% for term in site.glossary %}
  <details>
  <summary>

  <h1 style="float:right">{{ term.name }}</h1>
  </summary>

  Source: {{ term.page.name }}, path: {{ term.path }}
  [Page link]({{ term.url }})
  Content:
  {{ term.content }}
  ---
  </details>
{% endfor %}

## end render

This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.
