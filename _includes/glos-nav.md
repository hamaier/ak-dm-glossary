# Nav var list

base: {{site.github.baseurl}}
base-p: {{site.github.pageurl}}
page: {{page.url}}
layout.gh: {{ layout.glosshome }}
site.ham-glosshome: {{ site.ham-glosshome }}

## INCLUDE-INDEX = {{include.index}}

[A]({{site.github.baseurl}}/{{layout.glosshome}}#a) -
[B]({{site.github.baseurl}}/{{layout.glosshome}}#b) -
[M]({{site.github.baseurl}}/{{layout.glosshome}}#m) -
[Top]({{site.github.baseurl}}/{{layout.glosshome}})

{% assign varb = "A,B,C,D,J-P,M,N,O,P,Top" | split: "," %}

{% capture home %}
{{site.github.baseurl | append: '/'}}{{site.ham-glosshome}}
{% endcapture %}

{%- for item in varb -%}

[{{item}}]({{home}}#{{item | downcase}}) -

{%- endfor -%}


{%include show-debug.md%}
