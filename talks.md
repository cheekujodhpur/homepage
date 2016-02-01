---
layout: page
title: Talks
permalink: /talks/
---

<div class="posts">
    {% for post in site.categories.talks | sort: 'weight' reversed %}
        <a></a>
        <h3 class="link_blue">{{ post.title }}</h3>
        <h6>
        {{ post.organization }}<span style="color:red">.</span>&nbsp;&nbsp;{{ post.when }}<span style="color:red">.</span>
        </h6>
        {{ post.content }}
    {% endfor %}
</div>
