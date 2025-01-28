<h2 id="projects" class="section-title">Projects</h2>
<div class="projects-grid">
  {% for project in site.data.projects.main %}
  <div class="project-item">
    <div class="project-image">
      {% if project.image %}
      <img src="{{ project.image }}" alt="{{ project.title }}">
      {% endif %}
    </div>
    <div class="project-description">
      <h3><a href="{{ project.link }}" target="_blank">{{ project.title }}</a></h3>
      <p>{{ project.description }}</p>
    </div>
  </div>
  {% endfor %}
</div>

