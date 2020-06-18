---
layout: post
title:  "Obter Soma de Pontuação"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoes/obter-soma-pontuacao
pasta: "funcoes"
mainsection: 5.26
section: 5.263
---
# $FUNCAO_RETORNA_SOMA_PONTUACAO(NRQUESTAO...)
*Esta função está deprecada, utilizar **<a href="/fastQuestAdmin/funcoesv2/obterSomaPontuacao">Obter Soma Pontuação</a>***

*Recuperar a soma das pontuações de uma lista de questões.*
- Parâmetros:
    - NRQUESTAO..: Lista de identificador da questão separados por pipe "\|".
- Exemplo:
    - **$FUNCAO_RETORNA_SOMA_PONTUACAO(VERSAO\|LOOP\|OPER)**
- Resultado:
    - Irá retornar a soma da pontuação atribuida para as questões VERSAO,LOOP,OPER. caso nenhuma pontuação tenha sido atribuida irá retornar o valor -32791
