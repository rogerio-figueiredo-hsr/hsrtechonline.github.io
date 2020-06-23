---
layout: post
title:  "Principal"
projeto: "fastQuestColeta"
permalink: /fastQuestColeta/job-selecionado/principal
pasta: ""
mainsection: 2
section: 2.1
---

# Principal

---

### Tela principal

![Aba principal]({{ "/assets/img/coleta/aba-principal.png" | prepend: site.baseurl }}){:width="900px"}

---

1. Teste de Questionário: Ao clicar será feito o redirecionamento para a [página da pesquisa](/fastQuestColeta/questionario). Entrevistas feitas através desse botão são somente para testes, não serão contabilizadas e o cliente será descartado ao término.
2. Entrevista Anônima: Ao clicar será feito o redirecionamento para a [página da pesquisa](/fastQuestColeta/questionario). Caso o cliente não venha de uma listagem, não se possua nenhuma informação prévia do mesmo.
3. Poderá ter duas opções:
    - Entrevista Manual: Ao clicar buscará um contato disponível dentro do job e abrirá a [janela de entrevista manual](/fastQuestColeta/job-selecionado/principal/entrevista-manual).
    - Receber ligações: Ao clicar mudará o status do PABX para online e começará a [receber ligações](/fastQuestColeta/job-selecionado/principal/receber-ligacoes).

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