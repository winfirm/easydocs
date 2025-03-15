---
layout: null
permalink: /archive.md
---

# Archive

{% for file in site.static_files %}
{% if file.path contains 'docs/' and file.extname == '.md' %}
- [{{ file.name | replace: '.md', '' }}({{ file.modified_time | date:"%Y-%m-%d" }})](./#!docs/{{ file.name | uri_escape}})
{% endif %}
{% endfor %}
