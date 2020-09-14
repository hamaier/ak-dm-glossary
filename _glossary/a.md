---
name: A Terms
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

# New Term
Added this to check logical rendering.
{% if page.asup %}
  {% include_relative {{ page.asup }} %}
{% endif %}

# Archive Folder
a consistent file structure with use constraints and backup schedule that houses the definitive record of a project’s data resources. Products in the archive folder are the subject of metadata records and are the versions intended for use and dissemination. Contrast with working folder.

{% if page.bsup %}
  {% include_relative {{ page.asup }} %}
{% endif %}
