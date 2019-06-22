---

layout: lab
title: Lab
permalink: /lab/
---

{% for project in site.projects %}
  <div class="card">
    <a href="{{ project.project_url }}" target="_blank">
      <div class="container-card">
        <h3><b>{{ project.title }}</b></h3> 
        <p>{{ project.description }}</p> 
      </div>
    </a>
    <a href="{{ project.github_link }}" target="_blank" data-toggle="tooltip" data-placement="bottom" title="GitHub">
      <i class="fab fa-github-square"></i>
    </a>
  </div> 
{% endfor %}

