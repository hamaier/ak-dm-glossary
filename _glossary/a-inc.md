## Page "A" annotation include

Code sample:

{%raw%}

This works:
```
{%- capture anno-pageb -%}
{{ page.id | split: "/" | last | strip }}-inc.md
{%- endcapture -%}
```

More:
```
{% if page.bsup %}
{% capture anno-page %}
{{page.id | split: "/" | last}}-inc.md
{% endcapture %}
```
{%endraw%}
End code
