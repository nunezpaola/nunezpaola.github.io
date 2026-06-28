---
layout: default
title: "Inicio"
---

<section class="hero">
  <p class="eyebrow">señales · sistemas · decisiones bajo incertidumbre</p>
  <h1>Buscar ventaja donde el ruido parece total.</h1>
  <p>
    Soy Paola Nuñez. Acá documento cómo convierto ideas en sistemas que deciden solos:
    hipótesis, datos, validación fría y procesos que sobreviven cuando el mercado cambia.
    Sin demos lindas, solo lo que aguanta evidencia.
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
