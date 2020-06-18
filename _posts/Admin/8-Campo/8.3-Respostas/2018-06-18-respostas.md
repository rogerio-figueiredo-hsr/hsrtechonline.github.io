---
layout: post
title:  "Troca Resposta"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/campo/respostas
pasta: "Campo"
mainsection: 8
section: 8.3
---
# Troca resposta

Permite listar e manipular as respostas de um cliente.

---

## Menu troca resposta

<div class="row" markdown="1">
<div class="6u 12u$(small)" markdown="1">
3. Dentro do menu "Campo", ache a opção "Troca resposta" e clique;
</div>
<div class="6u 12u$(small)" markdown="1">
![Imagem de apoio 1]({{ "/assets/img/adicionar-resposta-01.png" | prepend: site.baseurl }})
</div>                               
</div>

---

## Tela

![Imagem de apoio 1]({{ "/assets/img/campo-resposta-tela.png" | prepend: site.baseurl }})

---

## Listando respostas do cliente

1. Preencha o campo "Cliente" com o código do cliente:
![Imagem de apoio 1]({{ "/assets/img/campo-resposta-campo-cliente.png" | prepend: site.baseurl }})

2. Clique no botão "Listar".
![Imagem de apoio 1]({{ "/assets/img/campo-resposta-botao-listar.png" | prepend: site.baseurl }})

3. Todas as respostas do cliente serão listadas no grid abaixo.
![Imagem de apoio 1]({{ "/assets/img/campo-resposta-listando-respostas.png" | prepend: site.baseurl }})

---

## Índice

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