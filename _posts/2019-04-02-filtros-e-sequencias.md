---
layout: post
title:  "Filtros e Sequências"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/filtrosSequencias
pasta: "funcoesv2"
---

# Filtros e Sequências

- Sintaxe:
  - **Sequência Numérica (numericSequence)**
    - Quando o filtro a ser passado dentro de um função for informado como sequência numérica, deve-se escrever conforme abaixo:
      - Exemplo:
      `RM("nrquestao").Selecionadas().Contem([1,2,3]) **(declarar a sequência entre colchetes separados por vírgula)**`
      `RM("nrquestao").Selecionadas().Contem([1]) **(também é válido)**`
  - **Literal Inteiro (IntegerLiteral)**
    - Quando o filtro a ser passado dentro de um função for informado como literal inteiro, deve-se escrever conforme abaixo:
      - Exemplo:
      `RM("nrquestao").Selecionadas().Contem(1)`
  - **Sequência Texto (StringSequence)**
    - Quando o filtro a ser passado dentro de um função for informado como sequência de texto, deve-se escrever conforme abaixo:
      - Exemplo:
      `Cotas(["C1","c2"]).Volume()` **(declarar a sequência entre colchetes, cada item entre aspas duplas e separados por vírgula)**`
  - **Literal Texto (StringLiteral)**
    - Quando o filtro a ser passado dentro de um função for informado como literal de texto, deve-se escrever conforme abaixo:
      - Exemplo:
      `RM("nrquestao")... **(declarar um único texto entre aspas duplas)**`
