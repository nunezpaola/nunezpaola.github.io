---
layout: default
title: "Inicio"
---

<section class="hero">
  <p class="eyebrow"></p>
<h1>Notas sobre agentes y sistemas que se pueden medir.</h1>
<p>
  Soy Paola Nuñez. Este sitio es un cuaderno público donde documento experimentos,
  decisiones de diseño, errores y aprendizajes sobre agentes de IA, automatización,
  y research técnico.
</p>
  <a class="cta" href="#posts">Leer los posts</a>
  <a class="ghost" href="{{ '/about/' | relative_url }}">About</a>
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
