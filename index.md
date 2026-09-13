---
layout: default
---

# Navigating America from the Bottom Up

This is my personal blog about navigating housing, employment, public assistance, community services, and everyday life in Butte County, California.

After spending many years navigating homelessness, housing, employment, and the systems that are supposed to help people move forward, I've accumulated a lot of experiences, observations, questions, and stories.

This isn't intended to be a formal organization or an official source of information. It is simply my perspective, based on what I have experienced and what I continue to learn along the way.

---

## Recent Posts

{% if site.posts.size > 0 %}
{% for post in site.posts %}
### [{{ post.title }}]({{ post.url | relative_url }})

{{ post.date | date: "%B %-d, %Y" }}

{{ post.excerpt }}

[Read more →]({{ post.url | relative_url }})

---

{% endfor %}
{% else %}
*There aren't any posts yet. Check back soon.*
{% endif %}

---

## About Me

I'm Scotty Franzyshen.

**Building • Fixing • Serving**

I've spent much of my life building things, fixing things, working with technology, helping people, and participating in my community. This blog is another way of doing that—by documenting what I see from a perspective that isn't always represented.

[More about me →]({{ "/about/" | relative_url }})

