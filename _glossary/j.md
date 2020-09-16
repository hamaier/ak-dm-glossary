---
glosindex: J-P
layout: glos-nav
---

# {{page.glosindex}}

{%capture iname%}
{{page.glosindex}}
{%endcapture%}

### j.md vars - no spaces:
  - iname: {{iname}}
  - glosindex: {{page.glosindex}}

---
# {% include glos-nav.md param=iname %}
---
{%include show-debug.md%}
