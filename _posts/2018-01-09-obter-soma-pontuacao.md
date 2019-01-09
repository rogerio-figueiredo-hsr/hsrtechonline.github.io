---
layout: post
title:  "Obter Soma de Pontuação"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoes/obter-soma-pontuacao
pasta: "funcoes"
---
# $FUNCAO_RETORNA_SOMA_PONTUACAO(NRQUESTAO...)
*Recupera a pontuação para uma determinada questão.*
- Parâmetros:
    - NRQUESTAO..: Lista de identificador da questão separados por pipe "|".
- Exemplo:
    - **$FUNCAO_RETORNA_SOMA_PONTUACAO(VERSAO|LOOP|OPER)**
- Resultado:
    - Irá retornar a soma da pontuação atribuida para as questões VERSAO,LOOP,OPER. caso nenhuma pontuação tenha sido atribuida irá retornar o valor -32791