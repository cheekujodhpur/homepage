---
layout: page
title: Projects
permalink: /projects/
heading: Projects
---

<div class="posts">
    {% assign posts = site.projects | sort:'weight' | reverse %}
    {% for post in posts %}
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <h6>
        {% for category in post.categories %}
           {% if category != "projects" %}
            {{ category }}<span style="color:red">.</span>&nbsp;&nbsp; 
           {% endif %}
        {% endfor %}
        </h6>
    {% endfor %}
</div>
