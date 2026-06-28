---
layout: default
title: "Inicio"
---

<section class="hero">
  <p class="eyebrow">Research notes · agentes · mercados</p>
  <h1>Experimentos técnicos sobre agentes, datos y sistemas.</h1>
  <p class="lead">
    Soy Paola Nuñez. Uso este sitio como cuaderno público para documentar pruebas,
    decisiones de diseño y aprendizajes sobre IA aplicada, automatización,
    market data y workflows reproducibles.
  </p>
  <div class="hero-actions">
    <a class="cta" href="#posts">Leer notas</a>
    <a class="ghost" href="{{ '/about/' | relative_url }}">About</a>
  </div>
</section>

<section class="topics" aria-label="Temas">
  <span>LLM agents</span>
  <span>market data</span>
  <span>automation</span>
  <span>technical research</span>
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
