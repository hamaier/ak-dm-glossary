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
