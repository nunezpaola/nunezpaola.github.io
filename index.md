---
layout: default
title: "Inicio"
---

<section class="hero">
  <p class="eyebrow">Research notes · agentes · sistemas</p>
  <h1>Make THIS CHEAP</h1>
  <p class="lead">
    Blog de experimentos técnicos sobre agentes, datos y sistemas. Uso este sitio como cuaderno para documentar pruebas, decisiones de diseño y aprendizajes sobre IA aplicada, automatización, evaluación de modelos y workflows reproducibles.
  </p>
  <div class="hero-actions">
    <a class="cta" href="#posts">Leer notas</a>
    <a class="ghost" href="{{ '/about/' | relative_url }}">About</a>
  </div>
</section>

<section class="topics" aria-label="Temas">
  <span>LLM agents</span>
  <span>evaluation</span>
  <span>automation</span>
  <span>research systems</span>
</section>

<section id="posts" class="post-list">
  <div class="section-heading">
    <p class="eyebrow">Archive</p>
    <h2>Últimos posts</h2>
  </div>
  <ul>
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%d/%m/%Y" }}</time>
      </li>
    {% else %}
      <li class="empty-state">Todavía no hay posts publicados.</li>
    {% endfor %}
  </ul>
</section>
