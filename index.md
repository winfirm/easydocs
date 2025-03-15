---
layout: null
permalink: /index.md
---

# Easy Docs

## Docs List

{% for file in site.static_files limit:20 %}
{% unless post.next %} 
{% if file.path contains 'docs/' and file.extname == '.md' %}
- [{{ file.name | replace: '.md', '' }}({{ file.modified_time | date:"%Y-%m-%d" }})](./#!docs/{{ file.name | uri_escape}})
{% endif %}
{% endunless %} 
{% endfor %}

[All documents &rarr;](./#!archive.md)

## Appendix

- EasyDocs powered by [Mdwiki-pro](https://github.com/winfirm/mdwiki-pro)
