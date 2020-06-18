---
layout: post
title:  "Tipos de Questões"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/cadastros/questionario/tipo-questao
pasta: "Cadastros"
mainsection: 5.2
section: 5.25
---
# Tipos de Questões

Os tipos de questões que podem ser cadastradas em um questionário.

<div>    
    {% assign sorted_threat_posts = site.posts | sort: 'section' %}  
    {% for post in sorted_threat_posts %}
        {%if post.projeto == "fastQuestAdmin" %}
            {%if post.mainsection == page.section %}  
            <ul  class="4u 6u$(small)">
                <li>
                    <a href="{{ site.baseurl}}{{ post.url}}">{{ post.title }}</a>  
                </li>
            </ul>
            {% endif %}
        {% endif %}
    {% endfor %}    
</div>     