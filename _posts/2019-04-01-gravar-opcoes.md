---
layout: post
title:  "Gravar Opções"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/gravarOpcoes
pasta: "funcoesv2"
---

# Gravar Opções
*Grava uma ou mais opções no banco para determinada questão informada*

- Sintaxe: 
  - `RM("NRQUESTAO").GravarOpcoes([OPCOES])`
- Parâmetros:
  - NRQUESTAO: Código da Questão (Texto entre aspas duplas) ou variável (sem aspas)
  - OPCOES: Códigos das opções numéricos entre colchetes separados por vírgula ou variável (sem aspas)
- Exemplo 1:
  - `RM("Q1").GravarOpcoes([1,2,3])`
- Exemplo 2:
  - <pre>
    <code>var nrquestao = (pode ser o retorno de uma função ou estático)
    var opcoes = (pode ser o retorno de uma função ou estático)
    RM(nrquestao ).GravarOpcoes(opcoes)</code>
    </pre>
