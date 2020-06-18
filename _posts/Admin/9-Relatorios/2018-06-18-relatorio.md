---
layout: post
title:  "Relatórios"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/relatorios
nomePasta: "Relatorio"
section: 9
---
# Relatórios

Neste menu teremos a opção de consultar e exportar informações e relatórios importantes
para a gestão do projeto.

<div>    
    {% assign sorted_threat_posts = site.posts | sort: 'section' %}  
    {% for post in sorted_threat_posts %}
        {%if post.projeto == "fastQuestAdmin" %}
            {%if post.pasta == page.nomePasta %} 
            <ul>
                <li>
                    <a href="{{ site.baseurl}}{{ post.url}}">{{ post.title }}</a>  
                </li>
            </ul>
            {% endif %}
        {% endif %}
    {% endfor %}    
</div>