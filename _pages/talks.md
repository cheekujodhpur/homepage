---
layout: page
title: Talks
permalink: /talks/
heading: Talks
---

<div class="posts">
    {% assign posts = site.talks | sort:'weight' | reverse %}
    {% for post in posts %}
        <a></a>
        <h3 class="link_blue">{{ post.title }}</h3>
        <h6>
        {{ post.organization }}<span style="color:red">.</span>&nbsp;&nbsp;{{ post.when }}<span style="color:red">.</span>
        </h6>
        {{ post.content }}
    {% endfor %}
</div>
