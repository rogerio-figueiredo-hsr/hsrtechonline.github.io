---
layout: post
title:  "Ocultar Questão"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/ocultarQuestao
pasta: "funcoesv2"
--- 

# Ocultar Questão
*Oculta uma ou mais questões conforme parâmetro informado na função "Questão"*
- Sintaxe: 
    - `Questionario().Questao(QUESTOES).Ocultar()`
- Parâmetros:
    - QUESTOES: Nomes das questões entre chaves em sequência literal entre aspas duplas separados por vírgula.
- Exemplo 1:
    - `Questionario().Questao([“Q1”,”Q2”,”Q3”]).Ocultar()`
- Exemplo 2:
    - <pre>
      <code>var param = (pode ser o retorno de uma função ou estático)
      Questionario().Questao(param).Ocultar()</code>
      </pre>
- Resultado:
    - Questões informadas serão ocultadas
