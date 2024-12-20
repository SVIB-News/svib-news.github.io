---
layout: archive
author_profile: true
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

-----

{% assign categories = "Issues,Articles" | split: "," %}

{% for category in categories %}
{% assign posts = site.posts | where_exp: "item", "item.categories contains category" | sort: "date" | reverse %}
## Recent {{ category }}
{% if posts.size > 0 %}
<div class="entries-list">
{% for post in posts limit:5 %}
{% include archive-single.html type=entries_layout %} 
{% endfor %}
</div>
{% else %}
<p>No {{ category | downcase }} found.</p>
{% endif %}
{% endfor %}
