---
title: "Introduction to Systems Development and Static Generators"
---

- Leer el capítulo 1 del libro _Developing Information Systems_ y resumir los conceptos clave, publicando el resumen como un post en un sitio web creado con Jekyll y GitHub Pages.

### Pasos a Seguir

1. **Instalación de Dependencias**

   - Ejecutar `bundle install` para instalar las gemas de Jekyll y el tema **Minimal Mistakes**.
   - Si hay problemas con la instalación, borrar `Gemfile.lock` y reinstalar.

2. **Visualización Local**

   - Ejecutar `rake serve` y acceder al sitio local en `http://127.0.0.1:4001/intro2sd-template/` para ver cambios en tiempo real.
   - Editar `_posts/2022-10-01-informe.md` y configurar el archivo `_config.yml` con información personal (autor, redes, etc.).

3. **Despliegue en GitHub Pages**

   - Configurar el `baseurl` en `_config.yml` con el nombre del repositorio.
   - Desplegar el sitio en la rama `gh-pages`.

4. **Despliegue Alternativo en Netlify y Vercel**

   - Cambiar el repositorio a público para el despliegue en Netlify.
   - Seguir las guías específicas para desplegar Jekyll en Netlify o Vercel.

5. **Personalización de la Página 404**

   - Crear una página 404 personalizada, usando un archivo `404.html` en la raíz del directorio `_site`.

6. **Entrega y Limpieza del Proyecto**
   - Eliminar posts de ejemplo y colecciones no propias.
   - Simplificar la navegación del sitio para incluir únicamente los contenidos relevantes de la práctica.

### Recursos Adicionales

- Documentación de Jekyll sobre páginas 404 personalizadas y configuración de despliegues en plataformas como Netlify y Vercel.
- Ejemplos de posts y colecciones en la guía de GitHub Pages para inspirarse al personalizar el perfil en GitHub.
