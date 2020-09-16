---
glosindex: J-P
layout: anno
nums: "A,B,C,D,E,F"
---
# {{glosindex}} use index

{% capture iname %}
{{glosindex}}
{% endcapture %}

{% include glos-nav.md index=iname %}
{%include show-debug.md%}
