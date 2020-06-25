# {{ site.url }}

# Try rendering glossary collection
{% for term in site.glossary %}
  # {{ term.name }}
  <p>{{ term.content | markdownify }}</p>

  ## raw content
  {{ term.content }}
  ### end of term
{% endfor %}

## end render

This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.
