---
name: nav-bar
layout:
nums: "A", "B", "C", "D", "E", "F"
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

{% assign varb = [1,2,3,4,5] %}

{% for item in varb %}
  {{ item }}
{% endfor %}

Top


{%include show-debug.md%}
