---
layout: default
title: "Browse Topics"
description: "Explore Scotty Franzyshen's essays by subject, from Chico housing and homelessness to community service, personal stories, and technology."
permalink: /topics/
---

# Browse by topic

Find related posts using the topic labels shown at the end of each article. These hashtags are website navigation ... they do not automatically publish anything to social media.

{% assign sorted_tags = site.tags | sort %}
{% for item in sorted_tags %}
{% assign topic = item[0] %}
{% assign posts_for_topic = item[1] | sort: 'date' | reverse %}
## <span id="{{ topic | slugify }}">#{{ topic | replace: ' ', '' }}</span>

{% for post in posts_for_topic %}
- [{{ post.title }}]({{ post.url | relative_url }}) ... {{ post.date | date: "%B %-d, %Y" }}
{% endfor %}

{% endfor %}

[Back to the blog]({{ '/' | relative_url }})
