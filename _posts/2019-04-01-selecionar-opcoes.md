---
layout: post
title:  "Selecionar Opção"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/selecionarOpcao
pasta: "funcoesv2"
---

# Selecionar()

- Sintaxe:
- Questões Múltiplas **(RM)**
  - Seleciona as opções declaradas na função **"Selecionar()"**
    - `RM("NRQUESTAO").Todas().Selecionar(OPCOES)`
- Questão Única **(RU)**
  - Seleciona a opçao declaradas na função **"Selecionar()"**
    - `RU("NRQUESTAO").Todas().Selecionar(OPCAO)`
- Parâmetros:
  - NRQUESTAO: Código da Questão (Texto entre aspas duplas) ou variável (sem aspas)
  - OPCOES: Códigos da opções numérico entre colchetes.
  - OPCAO: Código da opção numérico
- Exemplo 1:
  - `RM("Q1").Todas().Selecionar([1,2,3])`
  - `RU("Q1").Todas().Selecionar(1)`
- Exemplo 2:
    - <pre>
      <code>var opcoes = (pode ser o retorno númerico de uma função ou estático) ou
      var nrquestao = (pode ser o retorno de uma função ou estático)
      RM(nrquestao).Todas().Selecionar(opções)</code>
      </pre>
    - <pre>
      <code>var opcao = (pode ser o retorno de um único número de uma função ou estático)
      var nrquestao = (pode ser o retorno de uma função ou estático)
      RU(nrquestao).Todas().Selecionar(opcao)</code>
      </pre>
