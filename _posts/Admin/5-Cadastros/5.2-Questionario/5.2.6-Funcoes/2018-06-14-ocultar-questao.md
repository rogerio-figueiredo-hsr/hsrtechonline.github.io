---
layout: post
title:  "Ocultar Questão"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoes/ocultar-questao
pasta: "funcoes"
mainsection: 5.26
section: 5.2631
---
# $FUNCAO_EXECUTA_ACAO (OCULTARQUESTAO;VALOR)
*Esta função está deprecada, utilizar **<a href="/fastQuestAdmin/funcoesv2/ocultarQuestao">Ocultar Questão</a>***

Fará com que a questão não seja renderizada na página. Valor: NRQUESTAO
- Parametros: 
    - ACAO: OCULTARQUESTAO
    - VALOR: NRQUESTAO da questão que deseja ocultar
- Exemplo:
    - **$FUNCAO_EXECUTA_ACAO(OCULTARQUESTAO;Q11)**
- Resultado:
    - A questão Q11 não será mostrada na página do questionário
    
OU
## $FUNCAO_OCULTAR_QUESTAO (NRQUESTAO)
- Parâmetro:
    - NRQUESTAO: código da questao
- Exemplo:
    - **$FUNCAO_OCULTAR_QUESTAO(NRQUESTAO)**
