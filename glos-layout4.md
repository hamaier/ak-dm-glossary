---
layout: anno
testvar: lo4md
---
(glos-layout4.md) This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.

# glos-layout3.md using glossary layout in front matter
# Try rendering glossary collection
{% for term in site.glossary %}
# {{ term.name }}

---
### Source path: {{ term.path }} [Page link]({{ site.github.baseurl }}{{ term.url }})
---

## variables:
  - term.path: {{ term.path }}
  - term.relative_path: {{ term.path }}
  - term.url: {{ term.url }}
  - term.name: {{ term.name }}
  - site.url: {{ site.url }}
  - page.name: {{ page.name }}
  - page.path: {{ page.path }}
  - site.github.url: {{ site.github.url }}
  - site.github.baseurl: {{ site.github.baseurl }}
  - site.github.owner_name: {{ site.github.owner_name }}
  - site.github.owner_url: {{ site.github.owner_url }}
  - page.layout: {{page.layout}}
  - layout.myvar: {{layout.myvar}}

Content:
{{ term.content }}
---
{% endfor %}

## end render

This page was last updated at {{ "now" | date: "%Y-%m-%d %H:%M" }}.
