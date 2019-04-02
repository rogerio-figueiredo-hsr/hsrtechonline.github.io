---
layout: post
title:  "Retorna Menor Valor (Min)"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/min
pasta: "funcoesv2"
---
# Min()
*Retorna o menor valor entre as opções respondidas*

- Sintaxe: 
  - `SM(“NRQUESTAO”).Min()`
- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas
- Exemplo 1:
  - `1@10|2@20|3@30|4@0`
  - `SM(“Soma”).Min()`
- Exemplo 2:  
  - <pre>
    <code>var nrquestao: (pode ser o retorno de uma função ou estático)
    SM(nrquestao).Min()</code>
    </pre>
- Retorno:
  - 10
