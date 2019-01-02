---
layout: post
title:  "Resposta Única"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoes/resposta-unica
pasta: "funcoes"
---
# $FUNCAO_RESPOSTA_DUPLICADA(NRQUESTAO;VALOR_BUSCA;SOMENTE_REALIZADAS)
*Busca em uma determinada questão (NRQUESTAO) o valor passado na (VALOR_BUSCA).*
- Parâmetros:
    - NrQuestao: identificador da questão.
    - VALOR_BUSCA: valor a ser localizado
    - SOMENTE_REALIZADAS: passar (true) caso queira que a busca seja executada apenas em entrevistas realizadas, ou passar (false) para buscar em todas
- Exemplo:
    - **$FUNCAO_RESPOSTA_DUPLICADA(NOTA;$FUNCAO_RETORNA_RESPOSTA(NOTA);true)**
- Resultado:
    - Se houver uma outra resposta com o mesmo valor dado para a questão NOTA retorna 1 caso contrário retorna zero.