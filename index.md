---
layout: archive
author_profile: false
---

![SVIB News logo](/assets/images/logo-250x250.png)

# SVIB News

<small>SVIB news is designed to give students a voice in the school, offering unique content unprovided on the official platform.</small>

![Group photo](/assets/images/group-photo.jpg)

{% assign categories = "Issues,Articles" | split: "," %}

{% for category in categories %}
-----
{% include recents.html %}
{% endfor %}
