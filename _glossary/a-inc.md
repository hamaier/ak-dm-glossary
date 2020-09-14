## Page "A" annotation include (file a-inc.md)

Code sample:

{%raw%}

This works:
```
{%- capture anno-pageb -%}
{{ page.id | split: "/" | last | strip }}-inc.md
{%- endcapture -%}


{% include_relative {{ anno-pageb }} %}
```

So does this:
```
{% include_relative {{page.id | split: "/" | last}}-inc.md %}
```
{%endraw%}
