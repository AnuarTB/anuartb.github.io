---
layout: page
title: Projects
permalink: /projects/
---
<ul class="post-list">
{% for project in site.projects reversed %}
    <li>
        <h2>{{project.title}}</h2>
        <br/>
        <p>{{project.description}}</p>
        <div>
        {% if project.github_url %}
            <a href='{{ project.github_url }}' target='_blank'>GitHub</a>
            <br/>
        {% endif%}
        {% if project.demo_url %}
            <a href='{{ project.demo_url }}'>Demo</a>
        {% endif%}
        </div>
        <br/>
        <hr/>
    </li>
{% endfor %}
</ul>