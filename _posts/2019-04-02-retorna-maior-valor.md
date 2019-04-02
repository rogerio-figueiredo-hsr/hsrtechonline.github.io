---
layout: post
title:  "Retorna maior Valor (Max)"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/retornaMaiorValor
pasta: "funcoesv2"
---

# Max()
*Retorna o maior valor entre as opções respondidas*

- Sintaxe: 
  - `SM(“NRQUESTAO”).Max()`
- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas
- Exemplo 1:
  - `1@10|2@20|3@30|4@0`
  - `SM(“Soma”).Max()`
- Exemplo 2:
  - <pre>
    <code>var nrquestao = (pode ser o retorno de uma função ou estático)
    SM(nrquestao).Max()</code>
    </pre>
- Retorno:
  - 30
