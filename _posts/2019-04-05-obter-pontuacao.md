---
layout: post
title:  "Obter Pontuação"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/obterPontuacao
pasta: "funcoes"
---	

# Obter Pontuação
*Retorna a pontuação para uma determinada questão.*

- Sintaxe:
  - `Pontuacao().ObterPontuacao("NRQUESTAO")`
- Parâmetros:
  - NRQUESTAO: Código da questão entre aspas duplas ou variável
- Exemplo 1:
  - `Pontuacao().ObterPontuacao("Q1")`
- Exemplo 2:
  - <pre>
    <code>var nrquestao = (pode ser o retorno de uma função ou estático)
    Pontuacao().ObterPontuacao(nrquestao)</code>
    </pre>
- Resultado:
  - Retorna o valor da pontuação atribuido à questão declarada
  
