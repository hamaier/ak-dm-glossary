---
layout: default
---
# File: test-inc-d (doesn't work)
 - frontmatter = layout: default
 - include_relative ./inc-a.md
## Test of include below:
---
{% include_relative ./inc-a.md %}
---
### H3 after above include
