---
layout: post
title:  "Travar Opções"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/travarOpcoes
pasta: "funcoesv2"
---

# Travar()
*Trava as opções declaradas na função **"Travar"***

- Sintaxe:
- Questoes Multiplas **(RM)**
  - Trava as opções declaradas na função "Travar" retornadas da funçao **"Todas()"**
    - `<b>RM</b>("NRQUESTAO").Todas().Travar(OPCOES)`
  - Trava as opções declaradas na função "Travar" retornadas da funçao **"Selecionadas()"**
    - `<b>RM</b>("NRQUESTAO").<b>Selecionadas()</b>.Travar(OPCOES)`
  - Trava as opções declaradas na função "Travar" retornadas da funçao **"NaoSelecionadas()"**
    - `<b>RM</b>("NRQUESTAO").NaoSelecionadas().Travar(OPCOES)`
- Questao Única **(RU)**
    - Trava as opções declaradas na função "Travar" retornadas da funçao **"Todas()"**
      - `<b>RU</b>("NRQUESTAO").Todas().Travar(OPCOES)`
    - Trava a opçao declaradaa na função "Travar" retornada da funçao **"Selecionada()"**
      - `<b>RU</b>("NRQUESTAO").<b>Selecionada()</b>.Travar(OPCOES)`
    - Trava as opções declaradas na função "Travar" retornadas da funçao **"NaoSelecionadas()"**
      - `<b>RU</b>("NRQUESTAO").NaoSelecionadas().Travar(OPCOES)`
- Ranking **(RNK)**
  - **Não Implementado**
    - Trava as opções declaradas na função "Travar" retornadas da funçao **"Todas()"**
      - `<b>RNK</b>("NRQUESTAO").Todas().Travar(OPCOES)`
  - Trava as opções declaradas na função "Travar" retornadas da funçao **"Selecionadas()"**
    - `<b>RNK</b>("NRQUESTAO").<b>Selecionadas()</b>.Travar(OPCOES)`
  - Trava as opções declaradas na função "Travar" retornadas da funçao **"NaoSelecionadas()"**
    - `<b>RNK</b>("NRQUESTAO").NaoSelecionadas().Travar(OPCOES)`
- Somatoria **(SM)**
  - **Não Implementado**
    - Trava as opções declaradas na função "Travar" retornadas da funçao **"Todas()"**
      - `<b>SM</b>("NRQUESTAO").Todas().Travar(OPCOES)`
  - Trava as opções declaradas na função "Travar" retornadas da funçao **"Selecionadas()"**
    - `<b>SM</b>("NRQUESTAO").<b>Selecionadas()</b>.Travar(OPCOES)`
  - Trava as opções declaradas na função "Travar" retornadas da funçao **"NaoSelecionadas()"**
    - `<b>SM</b>("NRQUESTAO").NaoSelecionadas().Travar(OPCOES)`
  
- Parâmetros:
  - NRQUESTAO: Código da Questão (Texto entre aspas duplas) ou variável (sem aspas)
  - OPCOES: Códigos da opções numéricos entre colchetes
- Exemplo 1:
  - `<b>RM</b>("Q1").Todas().Travar([1])`
  - `<b>RU</b>("Q1").Todas().Travar([1])`
  - `<b>SM</b>("Q1").Selecionadas().Travar([1])`
  - `<b>RNK</b>("Q1").Selecionadas().Travar([1])`
- Exemplo 2:
    - <pre>
      <code>var opcoes = (pode ser o retorno de uma função ou estático)
      var nrquestao = (pode ser o retorno de uma função ou estático)
      <b>RM</b>(nrquestao).Todas().Travar(opções) ou <b>RU</b>(nrquestao).Todas().Travar(opções)</code>
      </pre>
