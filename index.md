---
layout: index
title: Hollyburn Sailing Club
---

## Posts

{% for post in site.posts %}
<dl class="dl-horizontal">
    <dt>
        <span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
    </dt>
    <dd>
        {{ post.content }}
    </dd>
</dl>
{% endfor %}

