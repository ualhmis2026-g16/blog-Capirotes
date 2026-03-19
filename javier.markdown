---
layout: page
title: "Javier Campuzano García"
permalink: /javier.html
---

<div style="display: flex; align-items: center; gap: 2rem; margin-bottom: 2rem;">
  <img src="{{ '/assets/img/avatar2.jpg' | relative_url }}" onerror="this.src='https://api.dicebear.com/7.x/avataaars/svg?seed=Javi'" style="width: 150px; height: 150px; border-radius: 50%; border: 4px solid var(--accent); object-fit: cover;">
  <div>
    <h1 style="margin: 0;">¡Hola! Soy Javier Campuzano García 👋</h1>
    <p style="font-size: 1.2rem; color: var(--text-secondary); margin: 0.5rem 0 0;">Ingeniero de Software y Tecnologías de la Información</p>
  </div>
</div>

---

## 🛠️ Mi Stack Tecnológico

| Categoría | Tecnologías |
| :--- | :--- |
| **Lenguajes** | ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=flat&logo=openjdk&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=flat&logo=c%2B%2B&logoColor=white) |
| **Herramientas** | ![Git](https://img.shields.io/badge/git-%23F05033.svg?style=flat&logo=git&logoColor=white) ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=flat&logo=docker&logoColor=white) ![Visual Studio Code](https://img.shields.io/badge/VS%20Code-007ACC?style=flat&logo=visual-studio-code&logoColor=white) |
| **Metodologías** | Scrum, Kanban, Test Driven Development (TDD) |

---

## 📫 Conecta conmigo
* 💼 [LinkedIn](https://www.linkedin.com/in/javier-campuzano-garc%C3%ADa-756755364/)
* 📧 jcampuzanog24@gmail.com

---

## 📝 Mis entradas en el blog
<div class="blog-feed">
{% assign javier_posts = site.posts | where: "author", "Javier" %}
{% for post in javier_posts %}
  <article class="post-card" style="margin-bottom: 1.5rem; padding: 1.5rem; border-radius: 12px; border: 1px solid var(--border-color);">
    <h4 style="margin: 0;"><a href="{{ post.url | relative_url }}" style="color: var(--accent); text-decoration: none;">{{ post.title }}</a></h4>
    <small style="color: #94a3b8;">{{ post.date | date: "%b %d, %Y" }}</small>
  </article>
{% endfor %}

{% if javier_posts.size == 0 %}
  <p>Aún no he publicado ninguna entrada. ¡Vuelve pronto!</p>
{% endif %}
</div>