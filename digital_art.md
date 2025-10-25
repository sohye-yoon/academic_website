---
layout: page
permalink: /digital_art/
I enjoy creating digital art in my spare time, focusing on minimalist compositions and portrait work.  
Below are a few selected pieces.

<br>

{% assign art = site.static_files | where_exp: "f", "f.path contains 'assets/artwork/'" %}
{% for image in art %}
  {% assign ext = image.extname | downcase %}
  {% if ext == ".jpg" or ext == ".jpeg" or ext == ".png" or ext == ".gif" or ext == ".webp" %}
    <figure style="display:inline-block; margin:0.5em;">
      <img src="{{ image.path | relative_url }}" alt="Digital artwork by So Hye Yoon" width="300" style="border-radius:8px;">
    </figure>
  {% endif %}
{% endfor %}

<br>
