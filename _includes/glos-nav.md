{%comment%}
  Generate index navigation bar entries.
  This include file should be called from a file in the
  collection, named such that it is rendered in the proper
  sorted location.
{%endcomment%}

{% assign varb = "A,B,C,D,J-P,M,N,O,P,Top" | split: "," %}

{% capture home %}
{{site.github.baseurl | append: '/'}}{{site.ham-glosshome}}
{% endcapture %}

{% assign delim = " " %}
{%for item in varb%}
[[{{item}}]({{home}}#{{item | downcase}})]{{delim}}
{%endfor%}

{% comment %}
{%include show-debug.md%}
{% endcomment %}
