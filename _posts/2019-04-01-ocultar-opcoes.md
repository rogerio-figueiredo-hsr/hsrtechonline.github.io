---
layout: post
title:  "Ocultar Opções"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/ocultarOpcoes
pasta: "funcoesv2"
---

# Ocultar()
*Oculta as opções declaradas na função **"Ocultar"***

- Sintaxe:
- Oculta as opções declaradas na função "Ocultar" retornadas da funçao **"Todas()"**
  - `RM("NRQUESTAO").Todas().Ocultar(OPCOES)`
- Oculta as opções declaradas na função "Ocultar" retornadas da funçao **"Selecionadas()"**
  - `RM("NRQUESTAO").Selecionadas().Ocultar(OPCOES)`
- Oculta as opções declaradas na função "Ocultar" retornadas da funçao **"NaoSelecionadas()"**
  - `RM("NRQUESTAO").NaoSelecionadas().Ocultar(OPCOES)`

- Parâmetros:
  - NRQUESTAO: Código da Questão (Texto entre aspas duplas) ou variável (sem aspas)
  - OPCOES: Códigos da opções numéricos entre colchetes
- Exemplo 1:
  - `RM("Q1").Todas().Ocultar([1])`
  - `RM("Q1").Selecionadas().Ocultar([1])`
  - `RM("Q1").NaoSelecionadas().Ocultar([1])`
- Exemplo 2:
    - <pre>
      <code>var opcoes = (pode ser o retorno de uma função ou estático)
      var nrquestao = (pode ser o retorno de uma função ou estático)
      RM(nrquestao).Todas().Ocultar(opções)</code>
      </pre>
