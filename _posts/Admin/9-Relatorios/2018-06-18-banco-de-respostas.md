---
layout: post
title:  "Banco de Respostas"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/relatorios/banco-de-respostas
pasta: "Relatorio"
mainsection: 9
section: 9.2
---
# Banco de Respostas

Neste submenu podemos exportar um banco de respostas de acordo com os critérios que
definirmos nos templates.
> Um template é um conjunto de "Status", "Campos de listagem" e "Questões" a qual se deseja gerar o relatório

<div class="row" markdown="1">
<div class="6u 12u$(small)" markdown="1">

1. Dentro do menu relatórios clique na opção "Banco de respostas".
</div>
<div class="6u 12u$(small)" markdown="1">
![Imagem de apoio 1]({{ "/assets/img/banco-de-respostas-01.png" | prepend: site.baseurl }})
</div>                               
</div>

{:start="2"}
2. A lista de templates irá aparecer.

3. Crie, altere ou exclua templates utilizando o botão novo, localizado na parte inferior da lista de templates.
![Lista de templates]({{ "/assets/img/BotoesListaTemplate.jpg" | prepend: site.baseurl }})

----
## Criar Templates
![Lista de templates]({{ "/assets/img/CriarNovoTemplate.jpg" | prepend: site.baseurl }})

1. Se sim, o relatório virá com a descrição das opções. Se não, o relatório virá com o valor das opções.  
2. Se sim, o relatório traz o tempo gasto com cada questão. Se não, o relatório traz as respostas.  
3. Selecione os status desejados   
4. Selecione as colunas desejadas
5. Selecione as questões
6. Finalize com o nome desejado do template

> O template fica gravado no projeto e acessível para todos os usuários que podem solicitar o relatório a qualquer momento  
> As solicitações podem ser imediatas ou agendadas com ou sem recorrência (podem repetir periodicamente)

![Solicitacao de Banco de respostas]({{ "/assets/img/SolicitacaoBancoResposta.jpg" | prepend: site.baseurl }})

1. Visualização do template por Status, Listagem e Questões.
2. Solicitação imediata de CSV
3. Solicitação de agendamento com ou sem repetição periódica de CSV
4. Solicitação imediata de SPS
5. Solicitação de agendamento com ou sem repetição priódica de SPSS
6. Permite consultar o tipo de periodicidade aplicado ao template, caso exista um.
> A imagem abaixo mostra a recorrencia de um template
![Lista recorrencias]({{ "/assets/img/ListaRecorrencia.png" | prepend: site.baseurl }})
> É possível remover a recorrência selecionando a linha e clicando na lixeira 

## Solicitar sem informar data
![Agendamento de banco de respostas]({{ "/assets/img/SolicitarRelatorioSemData.jpg" | prepend: site.baseurl }})

## Solicitar com data de inicio e fim
![Agendamento de banco de respostas]({{ "/assets/img/SolicitarRelatorioComData.jpg" | prepend: site.baseurl }})

## Agendar um relatório
![Agendamento de banco de respostas]({{ "/assets/img/SolicitarAgendamentoBancaoRespostaNaoRepete.jpg" | prepend: site.baseurl }})

1. Selecione o tipo de recorrência do agendamento, ou seja, de quanto em quanto tempo ele deve se repetir  
2. Selecione a data do primeiro evento
3. Selecione a hora do primeiro evento
4. Efetive o agendamento

Atualmente as opções de repetição são Diária e Semanal conforme imagem abaixo:

![Tipos de recorrência]({{ "/assets/img/TipoRecorrencia.jpg" | prepend: site.baseurl }})