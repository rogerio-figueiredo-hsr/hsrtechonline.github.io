---
layout: post
title:  "Lista Cotas Proporcional"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/cotas-proporcional
pasta: "funcoesv2"
---
# Proporcional
*Retorna uma lista com cotas que tem metas a serem cumpridas ordenadas pela cota menos cumprida até a cota mais próxima de cumprir*

- Sintaxe: 
  - `Cotas([COTAS]).Proporcional(QTDCOTAS)`
- Parâmetros:
  - **(Opcional)** COTAS: Lista de códigos de cotas entre aspas duplas e separados por vírgula.
  - **(Opcional)** QTDCOTAS: número que indica a quantidade de cotas.
  - Obs.: 
    - COTAS não informadas, representa que não filtrará as cotas retornadas
    - QTDCOTAS não informada, representa que não filtrará a quantidade.
- Exemplo 1: 
  - `Cotas().Proporcional()`
  - `Cotas(["C1","C2"]).Proporcional()`
  - `Cotas(["C1","C2"]).Proporcional(2)`
- Exemplo 2:
  - <pre>
    <code>var cotas = (pode ser o retorno de uma função ou estático)
    Cotas(cotas).Proporcional() ou 
    Cotas(cotas).Proporcional(2)</code>
    </pre>
- Resultado:
  - C1\|C2
