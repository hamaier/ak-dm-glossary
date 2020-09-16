---
glosindex: J-P
layout: anno
nums: "A,B,C,D,E,F"
---
# {{ page.glosindex }} use index

{% capture iname %}
{{ page.glosindex }}
{% endcapture %}

### j.md vars:
  - iname: {{ iname }}
  - glosindex: {{ page.glosindex }}



{% include glos-nav.md param=iname %}
{%include show-debug.md%}
