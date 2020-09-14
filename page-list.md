---
layout: draft
---
# List all pages (site.pages):
{% for page in site.pages %}
**page.name**: {{page.name}}, **URL**: {{page.url}}, **Path**: {{page.path}}
{% endfor %}


# List all documents in every collection (site.documents):
{% for page in site.documents %}
**page.name**: {{page.name}}, **URL**: {{page.url}}, **Path**: {{page.path}}
{% endfor %}


This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.
