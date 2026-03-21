---
layout: post
title: "Guía Práctica: Domina el flujo de trabajo en GitLab"
date: 2026-03-20 10:00:00 +0100
categories: gitlab tutorial
author: Victor
---

GitLab es una herramienta esencial para la colaboración en ingeniería. [cite_start]En este tutorial práctico, aprenderás desde configurar tu acceso hasta integrar cambios mediante Merge Requests[cite: 1, 2].

## 🔑 Paso 1: Configura tu llave SSH
[cite_start]Para conectar tu ordenador con GitLab de forma segura y sin pedir contraseña constantemente, usaremos llaves SSH[cite: 12].

1. **Genera la llave**: Abre una terminal y ejecuta:  
   [cite_start]`ssh-keygen -t ed25519 -C "tu-email@example.com"`[cite: 13].
2. [cite_start]**Copia la clave pública**: Usa el comando `type %USERPROFILE%\.ssh\id_ed25519.pub` (en Windows) y copia el contenido[cite: 14].
3. [cite_start]**Añádela a GitLab**: Ve a *User Settings* -> *SSH Keys* y pega tu clave[cite: 15].

## 📥 Paso 2: Clonar y Preparar el Proyecto
[cite_start]Una vez configurado Git con tu nombre y correo[cite: 20], es hora de traer el código a tu máquina:

* [cite_start]**Clonar**: Usa `git clone` seguido de la URL SSH de tu repositorio[cite: 24].
* [cite_start]**Sincronizar**: Entra en la carpeta y asegúrate de estar en la rama correcta con `git checkout tutorial` seguido de un `git pull`[cite: 25].


## 🚀 El Ciclo de Trabajo Diario
[cite_start]Para mantener el proyecto organizado, seguimos este flujo constante[cite: 70]:

### 1. Crear una Rama (Branch)
Nunca trabajes directamente en la rama principal. Crea una rama propia para tus tareas:
[cite_start]`git branch mi-rama` y luego `git checkout mi-rama`[cite: 49, 50].

### 2. Guardar Cambios (Commit & Push)
Cuando termines una tarea, guarda tus progresos:
* [cite_start]`git add .` (prepara los archivos)[cite: 35].
* [cite_start]`git commit -m "Descripción clara del cambio"`[cite: 36, 71].
* [cite_start]`git push origin mi-rama` (sube tus cambios a la nube)[cite: 53].

### 3. Mantenerse Actualizado (Pull)
Antes de empezar a trabajar, descarga siempre los cambios de tus compañeros para evitar conflictos:
[cite_start]`git pull origin tutorial`[cite: 44, 72].

## 🤝 Paso Final: El Merge Request
[cite_start]Cuando tu trabajo en la rama esté listo, es hora de unirlo al proyecto principal[cite: 65]:

1. [cite_start]Ve a **Merge Requests** en GitLab y crea uno nuevo[cite: 66].
2. [cite_start]Selecciona tu rama como *Source* y `tutorial` como *Target*[cite: 66].
3. [cite_start]**Revisión**: Asegúrate de marcar la opción de borrar tu rama personal tras el merge para mantener el repositorio limpio[cite: 67, 72].

---

> [cite_start]**💡 Consejo**: Haz commits a menudo (por ejemplo, después de cada sesión de laboratorio) para seguir mejor tu progreso[cite: 73].

¿Tienes dudas? [cite_start]No dudes en contactar conmigo o con cualquier miembro del equipo **ENG** durante las horas de prácticas[cite: 10]. ¡A darle caña al código!
