---
layout: post
title:  "Pular para página"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoes/pular-para-pagina
pasta: "funcoes"
mainsection: 5.26
section: 5.2637
---
# $FUNCAO_EXECUTA_ACAO (PAGINA;VALOR)
*Esta função está deprecada, utilizar **<a href="/fastQuestAdmin/funcoesv2/pularPagina">Pular para Página</a>***

Indica para qual página o questionário será redirecionado, valor: número da página

- Parametros: 
    - ACAO: **PAGINA**
    - VALOR: Número da página
- Exemplo:
    - **$FUNCAO_EXECUTA_ACAO(PAGINA;20)**
- Resultado:
 - Faz com que a próxima página a ser exibida seja a página 20. para exibir a página de uma determinada questão consulte a função $FUNCAO_PAGINA

OU

## $FUNCAO_PAGINA (NRQUESTAO)

- Parâmetros:
    - NRQUESTAO: codigio da questao desejada
- Exemplo:
    - **$FUNCAO_PAGINA(Q37)**
- Resultado
    - Localiza em que página a questão Q37 está e navega o questionário para esta página
