---
layout: default
avatar: true
permalink: /
---

## Recent Post
{% assign sortedPosts = site.posts | sort: 'date' | reverse %}
<ul>
{% for post in sortedPosts limit: 10 %}
    <li>
        <h2>
            <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
    <p class="description">
    {% if post.description %}
        {{ post.description | strip_html | strip_newlines | truncate: 250 }}
    {% else %}
        {{ post.content | strip_html | strip_newlines | truncate: 250 }}
    {% endif %}</p>
    </li>
{% endfor %} 
</ul>

