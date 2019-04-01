---
layout: post
title:  "Cotas"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/cotas
pasta: "funcoesv2"
---

# Em Andamento
*Coloca uma ou mais cotas em andamento*

- Sintaxe:
  - `Cotas([COTAS]).EmAndamento()`
- Parâmetros:
  - **(Opcional)** COTAS: Lista de códigos de cotas (entre aspas duplas e separados por vírgula
  - Obs.: COTAS não informadas, representa que não filtrará as cotas retornadas para colocá-las em Andamento
- Exemplo 1:
  - `Cotas().EmAndamento()`
  - `Cotas(["C1","C2"]).EmAndamento()`
- Exemplo 2:
  - <pre>
    <code>var cotas = (pode ser o retorno de uma função ou estático)
    Cotas(cotas).EmAndamento()</code>
    </pre>
- Resultado:
  - C1\|C2
