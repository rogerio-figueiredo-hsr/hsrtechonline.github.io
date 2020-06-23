---
layout: post
title: "Agendamentos/Retornos"
projeto: "fastQuestColeta"
permalink: /fastQuestColeta/job-selecionado/agendamentos-retorno
pasta: ""
mainsection: 2
section: 2.4
---

# Agendamentos/Retornos

Nesta aba serão listadas as entrevistas que foram agendadas para o entrevistador.

---

### Tela agendamentos/retornos

![Tela de agendamentos]({{ "/assets/img/coleta/tela-agendamento.png" | prepend: site.baseurl }}){:width="910px"}

---

1. **Ligar:** Clique no ícone <i class="fa fa-phone" style="color: #ff892a!important"></i> caso queira [efetuar uma ligação manual](/fastQuestColeta/job-selecionado/principal/entrevista-manual) para o cliente selecionado.
2. **CodCliente:** Código do cliente.
3. **Data:** Dia agendado para ligação.
4. **Hora:** Hora agendada para ligação.
5. **Contato do Agendamento:** Nome do cliente que teve a ligação agendada.
6. **Telefone Agendado:** Número do telefone agendado.
7. **Tipo:** Agendamento ou retorno.

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

