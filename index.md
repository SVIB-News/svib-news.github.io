---
layout: archive
author_profile: false
---

![Logo](/assets/images/logo.png){: .home-icon}

# Voice of Students

<small>Voice of Students is designed to give students a voice in the school, offering unique content unprovided on the official platform.</small>

![Group photo](/assets/images/group_photo.png)

{% assign categories = "Issues,Articles" | split: "," %}

{% for category in categories %}
-----
{% include recents.html %}
{% endfor %}
