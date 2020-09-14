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
  - No blank lines w/in if clause doesn't render properly
  - Blank line after if opening clause. doesn't render
  - Blank line before if closing clause. doesn't render
  - Blank line before start of if

{% if page.asup %}

  {% include_relative {{ page.asup }} %}

{% endif %}
(code used for above logical include)
	{% if page.asup %}
	  {% include_relative {{ page.asup }} %}
	{% endif %}
(end code)

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
{% capture name-only %}
{{page.name | remove: ".md"}}
{% endcapture %}

### Page.name trim: {{page.id | split: "/" | last}}-inc.md
### name-only: {{name-only}}"-inc"
{% endif %}
