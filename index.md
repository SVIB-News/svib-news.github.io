---
layout: archive
author_profile: false
---

![SVIB News logo](/assets/images/logo-250x250.png)

# SVIB News

<small>SVIB news is designed to give students a voice in the school, offering unique content unprovided on the official platform.</small>

-----

## Student Quotes

> I think the difficulty is mainly about no free time for writing it, but if I get to think of a interesting topic, it’s quite interesting after beginning.
>
> <small>Anabelle Wang</small>

> I felt good, because the experience not only helps me to pass my exams, but also taught me in a way that inspires curiosity, that sparks questions, that help me engage in the topic in a much deeper level.
>
> <small>Owen Gao</small>

{% assign categories = "Issues,Articles" | split: "," %}

{% for category in categories %}
    {% include recents.html %}
{% endfor %}
