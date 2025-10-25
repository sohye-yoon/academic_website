---
layout: page
permalink: /digital_art/
I enjoy creating digital art in my spare time, focusing on minimalist compositions and portrait work.  
Below are a few selected pieces.

<br>

{% for image in site.static_files %}
  {% if image.path contains 'assets/artwork/' %}
  <figure style="display:inline-block; margin:0.5em;">
    <img src="{{ image.path }}" alt="Digital artwork by So Hye Yoon" width="300" style="border-radius:8px;">
  </figure>
  {% endif %}
{% endfor %}

<br>
