---
layout: post
title:  "Questionário"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/cadastros/questionario
pasta: "Cadastros"
mainsection: 5
section: 5.2
---
# Questionário

Questionário é o local onde será adicionado as páginas, questões e condições sobre o projeto.

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