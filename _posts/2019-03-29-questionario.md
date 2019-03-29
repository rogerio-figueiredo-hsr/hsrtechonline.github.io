---
layout: post
title:  "Questionario"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/questionario
pasta: "questionario"
---
# Questionario

Funções são códigos pré desenvolvidos para a programação de questionários.
<div class="row">    
    {% for post in site.posts %}
        {%if post.projeto == "fastQuestAdmin" %}
            {%if post.pasta == page.nomePasta %}  
            <ul  class="4u 6u$(small)">
                <li>
                    <a href="{{ site.baseurl}}{{ post.url}}">{{ post.title }}</a>  
                </li>
            </ul>
            {% endif %}
        {% endif %}
    {% endfor %}    
</div>    
