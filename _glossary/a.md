---
name: nav-bar
layout: anno
---
# A - B -
C - D - O - Top

base: {{site.github.baseurl}}
base-p: {{site.github.pageurl}}
page: {{page.url}}
layout.gh: {{layout.glosshome}}

[A]({{site.github.baseurl}}/{{layout.glosshome}}#a) -
[B]({{site.github.baseurl}}/{{layout.glosshome}}#b) -
[M]({{site.github.baseurl}}/{{layout.glosshome}}#m) -
[Top]({{site.github.baseurl}}/{{layout.glosshome}})


{% for i in ["A", "B", "C", "D", "E", "F"] %}
  {{ i }} hello
{% endfor %}

Top


{%include show-debug.md%}
