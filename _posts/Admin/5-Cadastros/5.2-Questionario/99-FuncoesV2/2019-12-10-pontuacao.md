---
layout: post
title:  "Pontuação"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/pontuacao
pasta: "funcoesv2"
mainsection: 5.27
section: 5.281
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

# Obter Soma Pontuação
*Retorna a soma da pontuação para uma ou mais questões.*

- Sintaxe:
  - `Pontuacao().ObterSomaPontuacao([NRQUESTAOSEQUENCIA])`
- Parâmetros:
  - NRQUESTAOSEQUENCIA: Código das questões entre aspas duplas separadas por vírgula ou variável
- Exemplo 1:
  - `Pontuacao().ObterSomaPontuacao(["Q1","Q2"])`
- Exemplo 2:
  - <pre>
    <code>var nrquestao = (pode ser o retorno de uma função ou estático)
    Pontuacao().ObterSomaPontuacao(nrquestao)</code>
    </pre>
- Resultado:
  - Retorna o valor da soma da pontuação atribuido à(s) questão(ões) declarada(s)
  
  # Gravar Pontuação
*Atribui uma pontuação para uma determinada questão.*

- Sintaxe:
  - `Pontuacao().GravarPontuacao("NRQUESTAO","PONTUACAO")`
- Parâmetros:
  - NRQUESTAO: Código da questão entre aspas duplas ou variável
  - PONTUACAO: Valor decimal com (.) ponto entre aspas duplas ou variável
- Exemplo 1:
  - `Pontuacao().GravarPontuacao("Q1","5.5")`
- Exemplo 2:
  - <pre>
    <code>var nrquestao = (pode ser o retorno de uma função ou estático)
    var pontuacao = (pode ser o retorno de uma função ou estático)
    Pontuacao().GravarPontuacao(nrquestao,pontuacao)</code>
    </pre>
- Resultado:
  - Grava o valor declarado da pontuação atribuido à questão também declarada
