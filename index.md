---
layout: default
---

Choose a site below:

<ul class="nav nav-pills nav-stacked">
{% for nav in site.data.nav %}
    <li{% if page.url == nav.url %} class="active"{% endif %}><a href="{{ nav.url }}">{{ nav.text }}</a></li>
{% endfor %}
</ul>
