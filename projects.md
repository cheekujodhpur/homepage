---
layout: page
title: Projects
permalink: /projects/
---

<div class="posts">
    {% for post in site.categories.projects | sort: 'weight' reversed %}
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
