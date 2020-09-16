---
name: nav-bar
layout: default
---
# A - B - C - D - O - Top

base: {{site.github.baseurl}}
base-p: {{site.github.pageurl}}
page: {{page.url}}

[A]({{site.github.baseurl}}{{page.url}})#a
[B]({{site.github.baseurl}}{{page.url}})#b
[M]({{site.github.baseurl}}{{page.url}})#m
[Top]({{site.github.baseurl}}{{page.url}})

{%include show-debug.md%}
