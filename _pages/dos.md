---
layout: page
title: 75DOS
permalink: /75dos/
heading: 75 Days Of Summer
---

<div class="posts">
    {% assign dosposts = site.dos | sort:'weight' %}
        {% for post in dosposts %}
            <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
            <h6>
            {% for category in post.categories %}
               {% if category != "75dos" %}
                {{ category }}<span style="color:red">.</span>&nbsp;&nbsp; 
               {% endif %}
            {% endfor %}
            </h6>
        {% endfor %}
</div>
