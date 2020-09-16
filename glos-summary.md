---
layout: default
testvar: summary-only
tags: l3 t1
---
(glos-summary.md) This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.

Render "_glossary" collection using "default" layout and display only the "excerpt" of each file (current default is first paragraph). If additional content is available, a "View annotated definition" link is displayed.


{% for term in site.glossary %}

{% if term.glosindex %}
{{term.glosindex | prepend: "# " | markdownify}}

{% capture var1 %}
{{term.content | strip_newlines | prepend: "##"}}
{%endcapture%}

{% capture var2 %}
{{term.content | strip_newlines }}
{%endcapture%}

{{var1 | markdownify}}

{{var2 | markdownify | prepend: "##"}}


{%continue%}
{%endif%}

---
Source path: {{ term.path }} [Page link]({{ site.github.baseurl }}{{ term.url }})

{%comment%}
  Display variables for testing and debugging
  {%include show-debug.md%}
{%endcomment%}

# {{ term.term }}
{{ term.excerpt }}
{% if term.excerpt <> term.content %}
  View [annotated definition]({{ site.github.baseurl }}{{ term.url }})

{% endif %}

{% endfor %}

## end render

This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.
