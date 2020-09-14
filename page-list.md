---
layout: draft
---
# List all site pages:
{% for page in site.pages %}
**page.name**: {{page.name}}, *ID*: {{page.url}}, path: {{page.path}}
{% endfor %}

This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.
