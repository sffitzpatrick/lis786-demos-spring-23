---
title: Pully
layout: page
permalink: /pully
image_url: https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/PulleyShip.JPG/440px-PulleyShip.JPG
image_alt: This is some alt text
my_variable: This is some text that stands for a variable
---
{% include page-image.html %}
This is my page about Pullies!

{{ page.my_variable }}

{% for machine in site.machines %}
{% if machine.category == 'Pully' %}
<h3>{{ machine.title }}</h3>
<p><img src="{{ machine.image }}" alt="alt text here..." /></p>
<p>{{ machine.content }}</p>
<p>Category: {{ machine.category }}</p>
{% endif %}
{% endfor %}