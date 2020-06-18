---
layout: post
title:  "Dashboard"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/dashboard
nomePasta: "Dashboard"
section: 3
---
# Dashboard

O Dashboard é a primeira tela ao entrar em um Job, nela contem um resumo das entrevistas, segmentações, produtividade e cotas do job.

![Tela do Dashboard]({{ "/assets/img/dashboard-tela-inicial.png" | prepend: site.baseurl }})

---

## Alimentação Automática

![Alimentação do Job]({{ "/assets/img/dashboard-alimentacao.png" | prepend: site.baseurl }})

Aqui será exibido as filas que estão cadastradas e se estão ativas na alimentação automática ou não. 

- Para desabilitá-las basta clicar no botão SIM no final da linha da fila.
- No botão vermelho no canto direito superior você tem a opção de parar a alimentação automática, este botão desativa a alimentação, sendo assim, a alimentação só será novamente ativada se o botão "Iniciar" for clicado manualmente.

Na tela de alimentação do job podemos ver as seguintes informações a seguir:
- **Alimentação do job:** Mostra as filas automáticas dentro de cada projeto.
- **Situação:** indica a situação atual da alimentação do projeto uma lista das possíveis situações está descrita acima.
- **Data e hora da última execução:** indica a data e a hora em que a alimentação foi executada pela última vez.
- **Data e hora da próxima execução:** indica a data e hora em que a alimentação será executada novamente.
- **Número de registros:** indica a quantidade de registros na fila a serem executados.
- **Botão de ativação:** Você pode ativar ou desativar a próxima execução por fila clicando neste botão, sendo SIM para ativar e NÃO para desativar.

O serviço pode estar nas seguintes situações:
- **Aguardando Próxima Execução:** significa que o serviço está adormecido aguardando o horário da próxima execução.
- **Parado:** significa que a recuperação não está sendo executada e portando a alimentação está comprometida (Este serviço deve estar sempre sendo executado e não deve estar parado).
- **Executando:** significa que o serviço está sendo executado neste exato momento.
- **Falha:** significa que o serviço falhou e está parado esta situação deve ser informada imediatamente ao suporte técnico através do e-mail: atendimento@hsrtech.com.br

---

## Entrevistas

Neste grid é mostrado a quantidade de registros que possuímos classificados dentro de cada status. 

![Grid de entrevistas]({{ "/assets/img/dashboard-grid-entrevistas.png" | prepend: site.baseurl }})

1. Clique no canto superior direito no ícone de <i class="fa fa-file-excel-o" style="color: #428bca!important"></i> para exportar os dados do grid de entrevistas para um arquivo excel.
2. Grid de Entrevistas
 - **codStatus:** Código do status das entrevistas.
 - **Descrição:** Descrição do status das entrevistas.
 - **Quantidade:** Quantidade de entrevistas que possuem aquele status.
 - **Csv:** Clique no ícone <i class="fa fa-file-excel-o" style="color: #428bca!important"></i> para exportar para um arquivo excel todos os clientes no status da linha.

---

## Segmentação das listagens

Neste grid aparece a quantidade de entrevistas realizadas por segmentação da listagem e a
quantidade desejada cadastrada de acordo com o perfil do projeto.

![Grid de segmentações]({{ "/assets/img/dashboard-grid-segmentacoes.png" | prepend: site.baseurl }})

1. Clique no canto superior direito no ícone de <i class="fa fa-file-excel-o" style="color: #428bca!important"></i> para exportar os dados do grid de segmentações para um arquivo excel.
2. Grid de Segmentações
 - **Descrição:** Nome da segmentação.
 - **Realizado:** Quantidade de entrevistas realizadas na segmentação.
 - **Desejado:** Quantidade de entrevistas desejadas na segmentação. Caso não há um limite estipulado há quantidade será 0.
 - **Situação:** Quantos % faltam para bater a meta da segmentação. Caso tenha batido será exibido "atingiu!", caso não tenha estipulado um limite então será exibido "sem limite!".

---

## Cotas

Neste grid conseguimos auferir a quantidade de entrevistas realizadas x a cota e o % de atingimento das mesmas.

![Grid de cotas]({{ "/assets/img/dashboard-grid-cotas.png" | prepend: site.baseurl }})

1. Clique no canto superior direito no ícone de <i class="fa fa-file-excel-o" style="color: #428bca!important"></i> para exportar os dados do grid de cotas para um arquivo excel.
2. Grid de Cotas
 - **Descrição:** Nome da segmentação.
 - **Realizado:** Quantidade de entrevistas realizadas na cota.
 - **Desejado:** Quantidade de entrevistas desejadas na cota. Caso não há um limite estipulado há quantidade será 0.
 - **Situação:** Quantos % faltam para bater a meta da cota. Caso tenha batido será exibido "atingiu!", caso não tenha estipulado um limite então será exibido "sem limite!".

---

## Produtividade

Neste grid é possível verificar a produção diária, o tempo médio do questionário e a quantidade de
entrevistadores que tivemos trabalhando no projeto por dia e no total.

![Grid de produtividade]({{ "/assets/img/dashboard-grid-produtividade.png" | prepend: site.baseurl }})

1. Clique no canto superior direito no ícone de <i class="fa fa-file-excel-o" style="color: #428bca!important"></i> para exportar os dados do grid de produtividade para um arquivo excel.
2. Grid de Produtividade
 - **Data:** A data que as entrevistas foram realizadas.
 - **Realizada:** A quantidade de entrevistas realizadas naquela data.
 - **Tempo Médio:** O tempo médio de aplicação do questionário naquela data.
 - **Entrevistadores:** A quantidade de entrevistadores que trabalhou naquela data.




