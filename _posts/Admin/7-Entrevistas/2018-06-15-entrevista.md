---
layout: post
title:  "Entrevista"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/entrevista
nomePasta: "Entrevista"
section: 7
---
# Entrevista

Entrevista é o questionário que o cliente, no caso do CATI, responde para o entrevistador ou por meio de um CAWI onde responde um formulário recebido via e-mail.

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