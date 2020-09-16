---
glosindex: J-P
layout: anno
nums: "A,B,C,D,E,F"
---
# {{glosindex}} use index

{% capture iname %}
{{glosindex}}
{% endcapture %}

### j.md vars:
  - iname: {{iname}}
  - glosindex: {{glosindex}}



{% include glos-nav.md param=iname %}
{%include show-debug.md%}
