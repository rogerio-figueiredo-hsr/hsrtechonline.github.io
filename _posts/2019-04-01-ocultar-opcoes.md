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

- Sintaxe:
- Questoes Multiplas **(RM)**
  - Oculta as opções declaradas na função "Ocultar" retornadas da funçao **"Todas()"**
    - `<b>RM</b>("NRQUESTAO").Todas().Ocultar(OPCOES)`
  - Oculta as opções declaradas na função "Ocultar" retornadas da funçao **"Selecionadas()"**
    - `<b>RM</b>("NRQUESTAO").<b>Selecionadas()</b>.Ocultar(OPCOES)`
  - Oculta as opções declaradas na função "Ocultar" retornadas da funçao **"NaoSelecionadas()"**
    - `<b>RM</b>("NRQUESTAO").NaoSelecionadas().Ocultar(OPCOES)`
- Questao Única **(RU)**
    - Oculta as opções declaradas na função "Ocultar" retornadas da funçao **"Todas()"**
      - `<b>RU</b>("NRQUESTAO").Todas().Ocultar(OPCOES)`
    - Oculta a opçao declaradaa na função "Ocultar" retornada da funçao **"Selecionada()"**
      - `<b>RU</b>("NRQUESTAO").<b>Selecionada()</b>.Ocultar(OPCOES)`
    - Oculta as opções declaradas na função "Ocultar" retornadas da funçao **"NaoSelecionadas()"**
      - `<b>RU</b>("NRQUESTAO").NaoSelecionadas().Ocultar(OPCOES)`
  
- Parâmetros:
  - NRQUESTAO: Código da Questão (Texto entre aspas duplas) ou variável (sem aspas)
  - OPCOES: Códigos da opções numéricos entre colchetes
- Exemplo 1:
  - `<b>RM</b>("Q1").Todas().Ocultar([1])`
  - `<b>RU</b>("Q1").Todas().Ocultar([1])`
- Exemplo 2:
    - <pre>
      <code>var opcoes = (pode ser o retorno de uma função ou estático)
      var nrquestao = (pode ser o retorno de uma função ou estático)
      <b>RM</b>(nrquestao).Todas().Ocultar(opções) ou <b>RU</b>(nrquestao).Todas().Ocultar(opcoes)</code>
      </pre>
