---
title: A Terms
layout: default
asup: adi-inc.md
bsup: true
---
# Accessibility
the degree to which the resource is obtainable by an interested party. Direct access without constraint would be the most accessible (e.g. resources that may be downloaded without requiring a login), whereas resources that require third-party intervention would be less accessible.
{% include_relative acc-inc.md %}

# ADIwg
Alaska Data Integration working group
{% include_relative {{ page.asup }} %}

# New Term - no spaces
Added this to check logical rendering.
  - No blank line before if clause
  - Blank line after if clause
{% if page.asup %}
Inside the loop
{% include_relative {{ page.asup }} %}
{% endif %}

# Archive Folder
a consistent file structure with use constraints and backup schedule that houses the definitive record of a project’s data resources. Products in the archive folder are the subject of metadata records and are the versions intended for use and dissemination. Contrast with working folder.

{% if page.bsup %}
{% include_relative {{ page.asup }} %}
{% endif %}

(code used for above logical include)
	{% if page.bsup %}

	{% include_relative {{ page.asup }} %}
	{% endif %}
(end code)

# Page name logic
## page.name: {{page.name}}
## page.dir: {{page.dir}}
## page.path: {{page.path}}
## page.id: {{page.id}}

{% if page.bsup %}

{% capture anno-page %}
{{ page.id | split: "/" | last | strip }}-inc.md
{% endcapture %}

{%- capture anno2-page -%}
{{ page.id | split: "/" | last | strip }}-inc.md
{%- endcapture -%}

### Page.id trim: {{page.id | split: "/" | last}}-inc.md
### anno-page strip: {{- anno-page -}}
### anno2-page strip: {{ anno2-page }}

{% include_relative {{page.id | split: "/" | last}}-inc.md %}
{% endif %}
