---
layout: post
title:  "Entrevistas não finalizadas"
projeto: "fastQuestColeta"
permalink: /fastQuestColeta/job-selecionado/entrevistas-nao-finalizadas
pasta: ""
mainsection: 2
section: 2.5
---
# Entrevistas não finalizadas

Nesta tela serão listadas todas as entrevistas que o entrevistador iniciou porém foram interrompidas.

---

### Tela entrevistas não finalizadas

![Tela de entrevistas não finalizadas]({{ "/assets/img/coleta/tela-entrevistas-n-finalizadas.png" | prepend: site.baseurl }}){:width="910px"}

---

1. **Ligar:** Clique no ícone <i class="fa fa-phone" style="color: #ff892a!important"></i> caso queira [efetuar uma ligação manual](/fastQuestColeta/job-selecionado/principal/entrevista-manual) para o cliente selecionado.
2. **codCliente:** Código do cliente.
3. **codUsuario:** Código do entrevistador.
4. **codJob:** Código do projeto.
5. **CodStatus:** Código do status que o cliente está. 
6. **DescStatus:** Descrição do status do contato.
7. **Contato:** Nome do cliente.
8. **DDD1:** DDD do cliente. 
9. **Telefone1:** Telefone do cliente.

---

### Índice

<div>    
    {% assign sorted_threat_posts = site.posts | sort: 'section' %}  
    {% for post in sorted_threat_posts %}
        {%if post.projeto == "fastQuestColeta" %}
            {%if post.mainsection == page.section %}  
            <ul>
                <li>
                    <a href="{{ site.baseurl}}{{ post.url}}">{{ post.title }}</a>  
                </li>
            </ul>
            {% endif %}
        {% endif %}
    {% endfor %}    
</div>  
