---
layout: default
---

{% for resource in site.resources %}
<div class="post-preview">
    <div class="well">
    <h1><a href="{{ site.baseurl }}/{{ resource.permalink }}">{{ resource.title }}</a></h1>
    <div class="content">
      {{ resource.content | split:'<!--break-->' | first }}
    </div>
    <p><a href="{{ site.baseurl }}/{{ resource.permalink }}">Read More</a></p>
  </div>
</div>
{% endfor %}
