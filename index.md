---
layout: base.liquid
---

# hi. welcome to my blog.

I'm Erin. A Software Engineer currently working at ConvertKit. I write words about tech things like React, React Native, working remotely and other random things.

{% for post in collections.posts reversed %}
<a href="{{ post.url }}">
<h2>{{ post.data.title }}</h2>
<time>{{ post.data.date | date: "%B %d, %Y" }}</time>
</a>
{% endfor %}

<!-- npx @11ty/eleventy --serve -->
