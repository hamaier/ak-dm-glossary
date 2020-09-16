---
layout: default
testvar: lo4md
tag: l4 t1
---
(glos-layout4.md) This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.

# glos-layout4.md - render "_glossary" collection using "anno" layout

{% for term in site.glossary %}
---
### Source path: {{ term.path }} [Page link]({{ site.github.baseurl }}{{ term.url }})
---
# {{ term.name }}

{%comment%}
  Display variables for testing and debugging
{%endcomment%}

{%include show-debug.md%}

Collection.Content:
{{ term.content }}
---
{% endfor %}

## end render

This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.
