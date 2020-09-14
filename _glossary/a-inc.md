## Page "A" annotation include

Code sample:

```
{% if page.bsup %}
{% capture anno-page %}
{{page.id | split: "/" | last}}-inc.md
{% endcapture %}
```

End code
