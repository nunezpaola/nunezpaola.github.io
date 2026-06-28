---
layout: home
title: "Inicio"
---

<section class="hero">
  <p class="eyebrow"></p>
  <h1>Me divierten las cosas que funcionan solas.</h1>
  <p>
    Soy Paola Nuñez. En este blog documento ideas, resultados, errores, aprendizajes y procesos
    replicables aplicados a IA.
  </p>
  <a class="cta" href="#posts">Leer los posts</a>
</section>


<section id="posts" class="post-list">
  <h2>Ultimos posts</h2>
  <ul>
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span>{{ post.date | date: "%d/%m/%Y" }}</span>
      </li>
    {% endfor %}
  </ul>
</section>
