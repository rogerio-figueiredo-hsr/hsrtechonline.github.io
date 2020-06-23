---
layout: post
title:  "Dentro do Job"
projeto: "fastQuestColeta"
permalink: /fastQuestColeta/job-selecionado
nomePasta: "PaginaJobSelecionado"
section: 2
---
# Dentro do job

Após selecionar um Job algumas informações na tela serão recorrentes, como:

### Menu Superior

![Menu superior]({{ "/assets/img/coleta/barra-dentro-job.png" | prepend: site.baseurl }})

1. **Home:** Link de volta para a [tela de selecionar Jobs](/fastQuestColeta/jobs).
2. **SEU GRUPO:** Código e nome do grupo que o usuário está utilizando.
3. **JOB:** Nome do job selecionado.

---

### Abas

![Abas job]({{ "/assets/img/coleta/abas-dentro-job.png" | prepend: site.baseurl }})

Ao abrir um Job a aba inicial será sempre a [aba Principal](/fastQuestColeta/job-selecionado/principal)

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

---

### Status PABX
Caso o grupo do job que tenha selecionado esteja utilizando PABX, no canto inferior esquerdo da tela será exibido um ícone com o status que o PABX se encontra, eles podem ser: 

- **Offline:** Não está logado no PABX.
![Status Offline]({{ "/assets/img/receber-ligacoes-01.png" | prepend: site.baseurl }})

- **Paused:** Está logado no PABX porém não está procurando ligações, está pausado.
![Status Pausado]({{ "/assets/img/receber-ligacoes-02.png" | prepend: site.baseurl }})

- **Online:** Está pronto para receber ligações.
![Status Online]({{ "/assets/img/coleta/pabx-online.png" | prepend: site.baseurl }})

- **Ringing:** Está discando para algum contato.
![Status Onthephone]({{ "/assets/img/coleta/pabx-ringing.png" | prepend: site.baseurl }})

- **OnThePhone:** Está em uma ligação.
![Status Onthephone]({{ "/assets/img/coleta/pabx-onthephone.png" | prepend: site.baseurl }})

