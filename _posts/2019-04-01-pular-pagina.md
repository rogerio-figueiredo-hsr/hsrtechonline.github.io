---
layout: post
title:  "Pular Página"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/pularPagina
pasta: "funcoesv2"
---
# Pular Página
*Indica para qual página o questionário será redirecionado.*
- Sintaxe:
    - `Questionario().Pagina(PARAMETROS)`
- Parâmetros:
    - PARAMETROS: informar o número da página, o nome da questão entre aspas ou uma variável.
- Exemplo 1:
    - `Questionario().Pagina(1)`
    - `Questionario().Pagina(“Q1”)`
- Exemplo 2:
    - <pre>
      <code>var param = (pode ser o retorno de uma função ou estático)`
      Questionario().Pagina(param)</code>
      </pre>
- Resultado:
    - Questionário será redirecionado para a página/questão fornecida  
