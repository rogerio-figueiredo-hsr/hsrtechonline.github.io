---
layout: post
title:  "Somar Opções"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/somarOpcoes
pasta: "funcoesv2"
---

# Somar Opcoes
*Retorna a soma dos valores das opções informadas.*

- Sintaxe: 
  - `SM(“NRQUESTAO”).SomarOpcoes([OPCOES])}`
- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas
  - **(Opcional)** OPCOES: Sequência numérica informado com o numero das opções da questão.
- Exemplo 1: 
  - `SM(“Soma”).SomarOpcoes([1,2,3])`
- Exemplo 2: 
  - <pre>
    <code>var nrquestao = (pode ser o retorno de uma função ou estático)
    var opcoes = (pode ser o retorno de uma função ou estático)
    SM(nrquestao).SomarOpcoes(opcoes)</code>
    </pre>
- Retorno: 
  - A soma dos valores
