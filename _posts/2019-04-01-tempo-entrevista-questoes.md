---
layout: post
title:  "Cliente"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/cliente
pasta: "funcoesv2"
---
# Tempo Entrevista/Questoes
*Essa função Retorna o Tempo em segundos de duração da Entrevista e não recebe nenhum parâmetro de entrada.
Retorna a soma do tempo de uma questão/página ou mais.*

- Sintaxe:
    - Tempo da entrevista
        - `Cliente().TempoEntrevista()`
    - Tempo da(s) questão(õe)s ou página(s)
        - `Cliente().TempoEntrevista([SEQUENCIANUMERICA/SEQUENCIATEXTO])`
- Parâmetros:
    - SEQUENCIANUMERICA: paginas em sequência numérica separados por vírgula
    - SEQUENCIATEXTO: questões em sequência texto entre aspas duplas separados por vírgula
- Exemplo 1:
    - `Cliente().TempoEntrevista()`
    - `Cliente().TempoEntrevista([1,2,3])`
    - `Cliente().TempoEntrevista([“Q1”,”Q2”,”Q3”])`
- Exemplo 2:
    - <pre>
      <code>var paginas: (pode ser o retorno de uma função ou estático)
      Cliente().TempoEntrevista(paginas)</code>
      </pre>
- Exemplo 3:
    - <pre>
      <code>var questões: (pode ser o retorno de uma função ou estático)
      Cliente().TempoEntrevista(questoes)</code>
      </pre>
- Retorno:
    - Tempo em segundos
