---
layout: post
title:  "Questionário"
projeto: "fastQuestColeta"
permalink: /fastQuestColeta/questionario
nomePasta: "Questionario"
section: 3
---
# Questionário

É a página onde será aplicado a pesquisa.

---

### Cabeçalho do questionário
![Cabeçalho da coleta]({{ "/assets/img/coleta/cabecalho-pesquisa.png" | prepend: site.baseurl }})

1. **CodCliente:** Código do cliente que está respondendo a pesquisa.
2. **Contato:** Nome do cliente que está respondendo a pesquisa.
3. **DDD1:** DDD do cliente.
4. **Telefone1:** Telefone do cliente.
5. **Ocorrências:** Ao clicar abrirá uma janela que listará todas as ocorrências que o cliente teve. Pode ser acessado pressionando a tecla "F2".
6. **Campos Listagem:** Ao clicar abrirá uma janela que listará os campos da listagem do cliente. Pode ser acessado pressionando a tecla "F3".
7. **Troca de Contato:** Ao clicar abrirá uma janela onde você poderá [alterar o contato do cliente](/fastQuestColeta/questionario/trocando-contato). Pode ser acessado pressionando a tecla "F4".
8. **Encerrar:** Ao clicar abrirá a janela de encerramento que poder ser utilizada para [agendar](/fastQuestColeta/questionario/agendando-cliente) ou [encerrar](/fastQuestColeta/questionario/encerrando-cliente) o cliente. Pode ser acessado pressionando a tecla "F6".
9. **Salvar:** Ao clicar gravará as respostas da questões da página para que quando retomar não tenha que voltar para a página anterior.
10. **Tempo de Questionário:** Tempo total que o questionário está sendo aplicado.
11. **Tempo de Página:** Tempo que o entrevistador está na página.

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

---

### Visualizando campos de listagem do cliente

campos-listagem-cliente



