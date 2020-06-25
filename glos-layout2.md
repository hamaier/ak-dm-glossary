# Try rendering glossary collection
{% for term in site.glossary %}
  # {{ term.name }}
  Source: {{ page.neme }}, Page date: {{ page.date }}
  Content:
  {{ term.content }}
  ---
{% endfor %}

## end render

This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.
