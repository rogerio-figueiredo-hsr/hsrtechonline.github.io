---
layout: post
title:  "Tela Inicial"
projeto: "fastQuestColeta"
permalink: /fastQuestColeta/tela-inicial
nomePasta: "TelaInicial"
section: 0
---
# Acesso ao FastQuest Coleta

O endereço utilizado para acessar o módulo de coleta do FastQuest é <http://hsrtechonline.com.br/hsrtech/coleta/>.

---

### Tela inicial
![Tela Inicial]({{ "/assets/img/tela-inicial-tela.png" | prepend: site.baseurl }}){:width="700px"}

---

### Índice

<div>  
    {% assign sorted_threat_posts = site.posts | sort: 'section' %}  
    {% for post in sorted_threat_posts %}
        {%if post.projeto == "fastQuestColeta" %}
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