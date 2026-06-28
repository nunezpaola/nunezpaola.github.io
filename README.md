# Blog

Este sitio esta preparado con Jekyll para publicar experimentos con agentes.

## Estructura principal

- `_posts/`: articulos del blog.
- `_layouts/`: plantillas visuales.
- `assets/css/style.css`: estilos del sitio.
- `index.md`: portada y listado de posts.
- `_config.yml`: configuracion general.

### 1) Ejecutar localmente

Requiere Ruby y Bundler.

```bash
bundle install
bundle exec jekyll serve
```

Luego abrir: `http://127.0.0.1:4000`

### 2) Crear un nuevo post

Crear un archivo en `_posts/` con este formato de nombre:

`YYYY-MM-DD-titulo-del-post.md`

Ejemplo:

`2026-06-29-validacion-out-of-sample.md`

Plantilla base:

```md
---
layout: post
title: "Titulo del post"
date: 2026-06-29 10:00:00 -0300
categories: [blog]
tags: [quant-trading, research, agentes]
---

Introduccion.

## Hipotesis

## Metodo

## Resultados

## Riesgos y limites

## Proximos pasos
```

### 3) Publicar en GitHub Pages

1. commit y push a la rama `main`.
2. Esperar el build automatico.
