---
layout: default
testvar: summary-only
tags: l3 t1
---
(glos-summary.md) This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.

Render "_glossary" collection using "default" layout and display only the "excerpt" of each file (current default is first paragraph)


{% for term in site.glossary %}
---
Source path: {{ term.path }} [Page link]({{ site.github.baseurl }}{{ term.url }})
Var- glosindex: {{term.glosindex}}
{% if term.glosindex %}
{{term.glosindex}} is a separator
{%endif%}

{%comment%}
  Display variables for testing and debugging
  {%include show-debug.md%}
{%endcomment%}

{{ term.excerpt }}
View [annotated definition]({{ site.github.baseurl }}{{ term.url }})
{% endfor %}

## end render

This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.
