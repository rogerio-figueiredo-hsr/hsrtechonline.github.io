---
layout: post
title:  "Cadastro"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/usuario/gestao-usuario
pasta: "Usuarios"
mainsection: 2
section: 2.1
---
# Cadastro de usuários

### Menu cadastro

![Menu cadastro]({{ "/assets/img/cadastro-de-usuario-01.png" | prepend: site.baseurl }})

---

### Tela cadastro

Nesta tela será listado todos os usuários cadastrados no sistema.

![Imagem de apoio 1]({{ "/assets/img/usuario-cadastro-tela.png" | prepend: site.baseurl }})

---

### Índice
<div>    
    {% assign sorted_threat_posts = site.posts | sort: 'section' %}  
    {% for post in sorted_threat_posts %}
        {%if post.projeto == "fastQuestAdmin" %}
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