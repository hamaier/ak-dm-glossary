---
layout: draft
---
# List all site pages:
{% for page in site.pages %}
**page.name**: {{page.name}}, *ID*: {{page.id}}
{% endfor %}

This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.
