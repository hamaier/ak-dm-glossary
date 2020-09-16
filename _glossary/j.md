---
name: nav-bar
layout: anno
nums: "A,B,C,D,E,F"
---
# J-P
C - D - O - Top

base: {{site.github.baseurl}}
base-p: {{site.github.pageurl}}
page: {{page.url}}
layout.gh: {{ layout.glosshome }}
site.ham-glosshome: {{ site.ham-glosshome }}

[A]({{site.github.baseurl}}/{{layout.glosshome}}#a) -
[B]({{site.github.baseurl}}/{{layout.glosshome}}#b) -
[M]({{site.github.baseurl}}/{{layout.glosshome}}#m) -
[Top]({{site.github.baseurl}}/{{layout.glosshome}})

{% assign varb = "A,B,C,D,J-P,M,Top" | split: "," %}

{% capture home %}
{{site.github.baseurl | append: '/'}}{{layout.glosshome}}
{% endcapture %}

{%- for item in varb -%}

[{{item}}]({{home}}#{{item | downcase}}) -

{%- endfor -%}



{%include show-debug.md%}
