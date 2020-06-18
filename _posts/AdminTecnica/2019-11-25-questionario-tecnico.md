---
layout: post
title:  "Questionário"
projeto: "fastQuestAdminDocTec"
permalink: /fastQuestAdminDocTec/questionario
nomePasta: "questionario"
---
# Questionário

Neste tópico são discutidos tecnicamente o funcionamento do cadastramento e aplicação do questionário pela ferramenta de coleta

<div class="row">    
    {% for post in site.posts %}
        {%if post.projeto == "fastQuestAdminDocTec" %}
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