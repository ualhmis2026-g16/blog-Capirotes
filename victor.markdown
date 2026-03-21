---
layout: page
title: "Víctor Granero Reche"
permalink: /victor.html
---

<div style="text-align: center; margin-bottom: 3rem;">
  <img src="{{ '/assets/img/Victor.webp' | relative_url }}" onerror="this.src='https://api.dicebear.com/7.x/avataaars/svg?seed=Victor'" style="width: 180px; height: 180px; border-radius: 20px; border: 5px solid #2E86C1; object-fit: cover; box-shadow: 0 10px 20px rgba(0,0,0,0.1);">
  <h1 style="margin-top: 1.5rem; color: #2E86C1;">Víctor Granero Reche 🚀</h1>
  <p style="font-size: 1.3rem; color: #555; max-width: 600px; margin: 0.5rem auto;">Estudiante de 3º de Ingeniería Informática apasionado por la ingenieria del software</p>
</div>

---

## 💻 Mi ecosistema de desarrollo

| Ámbito | Tecnologías y Herramientas |
| :--- | :--- |
| **Core Dev** | ![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) |
| **Web & Data** | ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-CC0000?style=flat-square&logo=sqlite&logoColor=white) |
| **Workflow** | ![GitHub](https://img.shields.io/badge/GitHub-181717?style=social&logo=github) ![Markdown](https://img.shields.io/badge/Markdown-000000?style=social&logo=markdown) |

---

## 🤝 Contacto y Redes
Si quieres colaborar en algún proyecto o simplemente saludar, puedes encontrarme aquí:

* 📧 **Email UAL:** [vgr004@inlumine.ual.es](mailto:vgr004@inlumine.ual.es)
* 🐙 **GitHub:** [github.com/vgr004-ual](https://github.com/vgr004-ual)

---

## 📝 Mis publicaciones
En esta sección aparecerán mis aportaciones al **CapiBlogTe**:

<div class="blog-feed">
{% assign victor_posts = site.posts | where: "author", "Victor" %}
{% for post in victor_posts %}
  <article class="post-card" style="margin-bottom: 1.5rem; padding: 1rem; border-left: 4px solid #2E86C1; background: #f8f9fa;">
    <h4 style="margin: 0;"><a href="{{ post.url | relative_url }}" style="color: #2E86C1; text-decoration: none;">{{ post.title }}</a></h4>
    <small style="color: #666;">Publicado el {{ post.date | date: "%d/%m/%Y" }}</small>
  </article>
{% endfor %}

{% if victor_posts.size == 0 %}
  <p style="color: #999; font-style: italic;">Próximamente publicaré mis primeras guías técnicas. ¡Atentos!</p>
{% endif %}
</div>

---
[⬅️ Volver al Inicio]({{ site.baseurl }}/)