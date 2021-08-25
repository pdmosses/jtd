---
layout: default
permalink: /debug/
---

```json
{
  "jekyll": {{ jekyll.version | jsonify }},
  "hpages": [
    {%- for page in site.html_pages %}
    {%- if page.url == '/debug/' %}{% continue %}{% endif %}
    {
      "url"     : {{ page.url     | jsonify }},
      "name"    : {{ page.name    | jsonify }},
      "path"    : {{ page.path    | jsonify }},
      "title"   : {{ page.title   | jsonify }},
      "layout"  : {{ page.layout  | jsonify }},
      "content" : {{ page.content | jsonify }},
      "excerpt" : {{ page.excerpt | jsonify }}
    }{% unless forloop.last %},{% endunless -%}
    {% endfor %}
  ]
}
```
