---
layout: glossary
---
# Try rendering glossary collection
{% for term in site.glossary %}
  <details>
  <summary style="float:right">

  <h1>{{ term.name }}</h1>
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
