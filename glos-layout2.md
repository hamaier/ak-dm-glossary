# Try rendering glossary collection
{% for term in site.glossary %}
  <p>{{ term.content | markdownify }}</p>
{% endfor %}

## end render
