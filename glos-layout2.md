# {{ site.url }}

# Try rendering glossary collection
{% for term in site.glossary %}
  <h1>Get term name<h1>
  <h2>{{ term.name }}</h2>
  <p>{{ term.content | markdownify }}</p>
{% endfor %}

## end render
