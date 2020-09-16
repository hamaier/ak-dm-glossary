---
layout: default
testvar: summary-only
tags: l3 t1
---
(glos-summary.md) This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.

## Render "_glossary" collection using "default" layout and excerpt option to display only the first paragraph

{% for term in site.glossary %}
---
Source path: {{ term.path }} [Page link]({{ site.github.baseurl }}{{ term.url }})

{%comment%}
  Display variables for testing and debugging
  {%include show-debug.md%}
{%endcomment%}

{{ term.excerpt }}
View [annotated definition]({{ site.github.baseurl }}{{ term.url }})
{% endfor %}

## end render

This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.
