---
layout: post
title:  "Questionario"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/questionario
---
# Pular Página
*Indica para qual página o questionário será redirecionado.*
- Sintaxe:
    - Questionario().Pagina(PARAMETROS)
- Parâmetros:
    - NUMERO: informar o número da página.
    - NOME DA QUESTAO: informar o nome da questão.
- Exemplo:
    - **Questionario().Pagina(1)**
    - **Questionario().Pagina(“Q1”)**
- Resultado:
    - Questionário será redirecionado para a página/questão fornecida  

# Próxima Página
*Pula para a próxima página*
- Sintaxe: Questionario().ProximaPagina()
- Exemplo:
    - **Questionario().ProximaPagina()**
- Resultado:
    - Questionário pulará para a próxima página.
