---
layout: post
title:  "Segmentação"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/campo/segmentacao
pasta: "Campo"
mainsection: 8
section: 8.1
---
# Segmentação

Segmentação é uma divisão da listagem por meio de critérios definidos para o controle da ordem dos contatos a serem alimentados para o PABX.

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