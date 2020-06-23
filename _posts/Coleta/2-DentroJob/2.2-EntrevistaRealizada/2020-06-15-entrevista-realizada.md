---
layout: post
title:  "Entrevistas Realizadas"
projeto: "fastQuestColeta"
permalink: /fastQuestColeta/job-selecionado/entrevistas-realizadas
pasta: ""
mainsection: 2
section: 2.2
---
# Entrevistas realizadas

Nesta aba serão listadas todas as entrevistas que o entrevistador realizou.

---

### Tela entrevistas realizadas

![Tela entrevistas realizadas]({{ "/assets/img/coleta/tela-entrevistas-realizadas.png" | prepend: site.baseurl }}){:width="910px"}

---

1. **ID:** Código da entrevista realizada.
2. **Data:** Dia em que a entrevista foi realizada.
3. **Hora:** Hora em que a entrevista foi realizada.
4. **Nome do Cliente:** Nome do cliente que respondeu a pesquisa.

---

### Índice

<div>    
    {% assign sorted_threat_posts = site.posts | sort: 'section' %}  
    {% for post in sorted_threat_posts %}
        {%if post.projeto == "fastQuestColeta" %}
            {%if post.mainsection == page.section %}  
            <ul>
                <li>
                    <a href="{{ site.baseurl}}{{ post.url}}">{{ post.title }}</a>  
                </li>
            </ul>
            {% endif %}
        {% endif %}
    {% endfor %}    
</div>     