---
layout: post
title:  "Selecionar Opção"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/selecionarOpcao
pasta: "funcoesv2"
---

# Selecionar()

- Sintaxe:
  - Seleciona as opções declaradas na função **"Selecionar()"**
    - `RM("NRQUESTAO").Todas().Selecionar(OPCOES)`
- Parâmetros:
  - NRQUESTAO: Código da Questão (Texto entre aspas duplas) ou variável (sem aspas)
  - OPCOES: Códigos da opções numéricos entre colchetes
- Exemplo 1:
  - `RM("Q1").Todas().Selecionar(["1"])`
  - `RU("Q1").Todas().Selecionar(["1"])`
- Exemplo 2:
    - <pre>
      <code>var opcoes = (pode ser o retorno de uma função ou estático)
      var nrquestao = (pode ser o retorno de uma função ou estático)
      RM(nrquestao).Todas().Selecionar(opções) ou RU(nrquestao).Todas().Selecionar(opcoes)</code>
      </pre>
