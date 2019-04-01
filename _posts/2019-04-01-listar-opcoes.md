---
layout: post
title:  "Listar Opções"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/listarOpcoes
pasta: "funcoesv2"
---

# Opcoes()
*Lista as opções declaradas na função "Opcoes()"*

- Sintaxe:
- Lista as opções declaradas na função "Travar" retornadas da funçao "Todas()"
  - `RM("NRQUESTAO").Todas().Travar(OPCOES)`
- Trava as opções declaradas na função "Travar" retornadas da funçao "Selecionadas()"
  - `RM("NRQUESTAO").Selecionadas().Travar(OPCOES)`
- Trava as opções declaradas na função "Travar" retornadas da funçao "NaoSelecionadas()"
  - `RM("NRQUESTAO").NaoSelecionadas().Travar(OPCOES)`

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
