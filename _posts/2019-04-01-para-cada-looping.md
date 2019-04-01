---
layout: post
title:  "Para Cada (Loop)"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/paraCada
pasta: "funcoesv2"
---

# ParaCada()
*Trava as opções declaradas na função "Travar"*

- Sintaxe:


- Parâmetros:
  - NRQUESTAO: Código da Questão (Texto entre aspas duplas) ou variável (sem aspas)
  - OPCOES: Códigos da opções numéricos entre colchetes
- Exemplo 1:
  - `RM("Q1").Todas().Travar([1])`
  - `RM("Q1").Selecionadas().Travar([1])`
- Exemplo 2:
    - <pre>
      <code>var opcoes = (pode ser o retorno de uma função ou estático)
      var nrquestao = (pode ser o retorno de uma função ou estático)
      RM(nrquestao).Todas().Travar(opções)</code>
      </pre>
