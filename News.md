---
layout: page
title: news archive
permalink: /news/
---



{% for post in site.posts %}
<p class="post-meta">{{ post.date | date: '%B %-d, %Y' }}, <a href="{{ post.url | prepend: site.baseurl }}"> <b>{{post.title}}</b></a></p>
<p class="post-meta"> {{ post.description }}</p>
<br>
{% endfor %}









<!-- {% for image in site.static_files %}

    {% if image.path contains 'phds' %}

    <img class="one left" alt="Principal Investigator" width="25%" height="25%" src="{{ site.baseurl }}{{ image.path }}" >
    <p><b>Ahmad Rafsanjani</b>, Associate Professor at the Center for Soft Robotics, SDU Biorobotics</p>

    {% endif %}

{% endfor %} -->



<!-- {% for project in site.portfolio %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %} -->
