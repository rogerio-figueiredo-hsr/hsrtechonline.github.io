---
layout: post
title:  "Cotas"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/cotas
pasta: "funcoesv2"
---

# Volume
*Retorna uma lista com cotas que tem metas a serem cumpridas ordenadas pelo volume da cota menos realizada até a cota mais realizada*

- Sintaxe:
  - `Cotas(COTAS).Volume(QTDCOTAS)`
- Parâmetros:
  - **(Opcional)** COTAS: Lista de códigos de cotas entre aspas duplas e separados por vírgula
  - **(Opcional)** QTDCOTAS: número que indica a quantidade de cotas
  - Obs.: 
      - COTAS não informadas, representa que não filtrará as cotas retornadas
      - QTDCOTAS não informada, representa que não filtrará a quantidade.
- Exemplo 1: 
  - `Cotas().Volume()
  - `Cotas(["C1","C2"]).Volume()`
  - `Cotas(["C1","C2"]).Volume(2)`
- Exemplo 2:
  - <pre>
    <code>var cotas = (pode ser o retorno de uma função ou estático)
    Cotas(cotas).Volume()
    Cotas(cotas).Volume(2)</code>
    </pre>
- Resultado:
  - C1\|C2\
