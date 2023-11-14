---
title:
layout: default
permalink: /projects_copy/
published: true
---


<div class="ProjectContainer">

	<div class="gallery">


  {% for project in site.projects %}

  {% if project.redirect %}
  <div class="projectTile">
          <a href="{{ project.redirect }}" target="_blank">
          <span>
              <h2>{{ project.title }}</h2>
              <br/>
	      <img src="{{ project.descImg }}"/>
          </span>
          </a>
  </div>

  {% else %}

  <div class="projectTile">
          <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
          <span>
              <h2>{{ project.title }}</h2>
              <br/>
	      <img src="{{ project.descImg }}"/>
          </span>
          </a>
  </div>

  {% endif %}

  {% endfor %}

	</div>

</div>
