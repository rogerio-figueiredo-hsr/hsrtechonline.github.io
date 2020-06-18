---
layout: post
title:  "Tela Inicial"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/tela-inicial
nomePasta: "TelaInicial"
section: 0
---
# Acesso ao FastQuest

O endereço utilizado para acessar o módulo administrativo do FastQuest é <https://hsrtechonline.com.br/hsrtech/admin/>.

---

### Tela inicial
![Tela Inicial]({{ "/assets/img/tela-inicial-tela.png" | prepend: site.baseurl }})

---

### Índice

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