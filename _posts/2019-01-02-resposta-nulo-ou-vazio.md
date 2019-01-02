---
layout: post
title:  "Resposta Nulo ou Vazio"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoes/resposta-nulo-ou-vazio
pasta: "funcoes"
---
# $FUNCAO_RESPOSTA_NULO_OU_VAZIO(NRQUESTAO)
*Verifica se uma determinada questão foi ou não preenchida.*
- Parâmetros:
    - NrQuestao: identificador da questão.
- Exemplo:
    - **$FUNCAO_RESPOSTA_NULO_OU_VAZIO(NOTA)**
- Resultado:
    - Se a questão NOTA não tem resposta, retorna 1, caso contrário retorna 0 (zero).