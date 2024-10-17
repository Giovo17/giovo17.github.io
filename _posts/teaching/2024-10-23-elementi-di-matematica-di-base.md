---
layout: post
title: AA 24/25 Elementi di Matematica di base - Scienze del Turismo
categories: teaching
permalink: teaching/elements-of-basic-maths-aa2425
id: 2024-10-23-elementi-di-matematica-di-base
---


- id: prova-basic-maths
  description: Lezione 1 Elementi di matematica di base AA 24/25  # not shown
  small-description: Link
  color: "#ba2818"
  class: "far fa-file-pdf icon"
  url: "/files/teaching/2024-10-23-elementi-di-matematica-di-base/prova.pdf"
  on-homepage: false
  course-id: 2024-10-23-elementi-di-matematica-di-base
  document-type: slides
  lesson: 1


Elementi di Matematica di base - Scienze del Turismo

Anno accademico 24/25

<!--more-->


| Lezione         | Argomenti           | Data - Ora            | Slides          | Esercizi proposti |
| :-------:       | ------------------  | ---------------       | :-------:       | :-------:         |
| **Lezione 1**   | - Funzioni  <br>  - Funzioni nel piano cartesiano  | 23 Ottobre 2024 - 15.00/18.00   | 
{% for document in site.data.teaching-material %}
  {% if document.document-type == "slides" and document.course-id == page.id and document.lesson == 1 %}
    {% include teaching-document.html document=document %}
  {% endif %}
{% endfor %}    | 
{% for document in site.data.teaching-material %}
  {% if document.document-type == "exercises" and document.course-id == page.id and document.lesson == 1 %}
    {% include teaching-document.html document=document %}
  {% endif %}
{% endfor %}    |

| **Lezione 2**   | - Derivate  <br>  - Massimi, minimi e flessi  | 24 Ottobre 2024 - 15.00/18.00     |
{% for document in site.data.teaching-material %}
  {% if document.document-type == "slides" and document.course-id == page.id and document.lesson == 2 %}
    {% include teaching-document.html document=document %}
  {% endif %}
{% endfor %}    | 
{% for document in site.data.teaching-material %}
  {% if document.document-type == "exercises" and document.course-id == page.id and document.lesson == 2 %}
    {% include teaching-document.html document=document %}
  {% endif %}
{% endfor %}    |




