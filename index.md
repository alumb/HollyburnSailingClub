---
layout: index
title: Hollyburn Sailing Club
link_bar:
    - name: Home
      href: /
      class: active
    - name: About
      href: about
    - name: Sailing
      href: sailing
    - name: Kayaking
      href: kayaking
    - name: Club House
      href: club
    - name: Contact
      href: contact
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

