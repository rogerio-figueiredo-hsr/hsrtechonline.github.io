---
layout: post
title:  "Resposta Nulo ou Vazio"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoes/resposta-nulo-ou-vazio
pasta: "funcoes"
mainsection: 5.26
section: 5.2652
---
# $FUNCAO_RESPOSTA_NULO_OU_VAZIO(NRQUESTAO)
*Esta função está deprecada, utilizar **<a href="/fastQuestAdmin/funcoesv2/listarOpcoes">Listar Opções</a>***

*Verifica se uma determinada questão foi ou não preenchida.*
- Parâmetros:
    - NrQuestao: identificador da questão.
- Exemplo:
    - **$FUNCAO_RESPOSTA_NULO_OU_VAZIO(NOTA)**
- Resultado:
    - Se a questão NOTA não tem resposta, retorna 1, caso contrário retorna 0 (zero).
