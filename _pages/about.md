---
permalink: /about/
title: "About"
last_modified_at: 2024-11-10T00:00:00-00:00
toc: true
---

En esta práctica se personaliza un sitio web generado usando Jekyll. En este se añaden posts y colecciones personalizadas con el objetivo de probar el funcionamiento de distintas herramientas. También se lleva a cabo el despliegue del sitio haciendo uso de distintos servicios. Se utiliza el tema Minimal Mistakes, cuyos créditos aparecen al final de está página.

## Rúbrica

<ul>
{% for item in site.data.rubric.rubric %}
    <li style="list-style: none;">
        <input type="checkbox" id="checkbox-{{ item.number }}" {% if item.done %} checked {% endif %} disabled>
        <span>{{ item.criteria }}</span>
    </li>
{% endfor %}
</ul>

## Posts

| Nombre                                                         | Descripción                                                                                                 |
| -------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| [Informe de la práctica][report-post]                          | Informe de la práctica "Introduction to Systems Development" and Static Generators.                         |
| [Resumen "Introduction to Systems Development"][abstract-post] | Resumen del capítulo 1 del libro "Developing Information Systems: Practical Guidance for IT Professionals". |

[report-post]: {{ "" | relative_url }}{% post_url 2022-10-01-informe %}
[abstract-post]: {{ "" | relative_url }}{% post_url 2024-11-10-chapter1-abstract %}

---

## Créditos

### Icons + Demo Images:

- [The Noun Project](https://thenounproject.com) -- Garrett Knoll, Arthur Shlain, and [tracy tam](https://thenounproject.com/tracytam)
- [Font Awesome](http://fontawesome.io/)
- [Unsplash](https://unsplash.com/)

### Other:

- [Jekyll](https://jekyllrb.com/)
- [jQuery](https://jquery.com/)
- [Susy](http://susy.oddbird.net/)
- [Breakpoint](http://breakpoint-sass.com/)
- [Magnific Popup](http://dimsemenov.com/plugins/magnific-popup/)
- [FitVids.JS](http://fitvidsjs.com/)
- Greedy Navigation - [lukejacksonn](https://codepen.io/lukejacksonn/pen/PwmwWV)
- [jQuery Smooth Scroll](https://github.com/kswedberg/jquery-smooth-scroll)
- [Lunr](http://lunrjs.com)

Minimal Mistakes is designed, developed, and maintained by Michael Rose. Just another boring, tattooed, designer from Buffalo New York.
