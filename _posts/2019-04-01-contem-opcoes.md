---
layout: post
title:  "Verifica Opções (Contem)"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/contemOpcoes
pasta: "funcoesv2"
---

# Contem()
*Verifica se contém as opções declaradas na função **"Contem()"***

- Sintaxe:
- Questoes Multiplas **(RM)**
  - Verifica se contém as opções declaradas na função "Contem" na lista de opções retornadas da funçao **"Todas()"**
    - `RM("NRQUESTAO").Todas().Contem(OPCOES)`
  - Verifica se contém as opções declaradas na função "Contem" na lista de opções retornadas da funçao **"Selecionadas()"**
    - `RM("NRQUESTAO").Selecionadas().Travar(OPCOES)`
  - Verifica se contém as opções declaradas na função "Contem" na lista de opções retornadas da funçao **"NaoSelecionadas()"**
    - `RM("NRQUESTAO").NaoSelecionadas().Travar(OPCOES)`
- Questoes Multiplas **(RU)**
  - Verifica se contém as opções declaradas na função "Contem" na lista de opções retornadas da funçao **"Todas()"**
    - `RU("NRQUESTAO").Todas().Contem(OPCOES)`
  - Verifica se contém as opções declaradas na função "Contem" na lista de opções retornadas da funçao **"NaoSelecionadas()"**
    - `RU("NRQUESTAO").NaoSelecionadas().Contem(OPCOES)`
- **Não Implementado**
  - Ranking **(RNK)**
    - Trava as opções declaradas na função "Contem" retornadas da funçao **"Todas()"**
      - `<b>RNK</b>("NRQUESTAO").Todas().Contem(OPCOES)`
    - Trava as opções declaradas na função "Contem" retornadas da funçao **"Selecionadas()"**
      - `<b>RNK</b>("NRQUESTAO").<b>Selecionadas()</b>.Contem(OPCOES)`
    - Trava as opções declaradas na função "Contem" retornadas da funçao **"NaoSelecionadas()"**
      - `<b>RNK</b>("NRQUESTAO").NaoSelecionadas().Contem(OPCOES)`
  - Somatoria **(SM)**
    - Trava as opções declaradas na função "Contem" retornadas da funçao **"Todas()"**
      - `<b>SM</b>("NRQUESTAO").Todas().Contem(OPCOES)`
    - Trava as opções declaradas na função "Contem" retornadas da funçao **"Selecionadas()"**
      - `<b>SM</b>("NRQUESTAO").<b>Selecionadas()</b>.Contem(OPCOES)`
    - Trava as opções declaradas na função "Contem" retornadas da funçao **"NaoSelecionadas()"**
      - `<b>SM</b>("NRQUESTAO").NaoSelecionadas().Contem(OPCOES)`

- Parâmetros:
  - NRQUESTAO: Código da Questão (Texto entre aspas duplas) ou variável (sem aspas)
  - OPCOES: Códigos da opções numéricos entre colchetes
- Exemplo 1:
  - `RM("Q1").Todas().Contem([1])`
  - `RU("Q1").Todas().Contem([1])`
- Exemplo 2:
    - <pre>
      <code>var opcoes = (pode ser o retorno de uma função ou estático)
      var nrquestao = (pode ser o retorno de uma função ou estático)
      <b>RM</b>(nrquestao).Todas().Contem(opcoes) ou <b>RU</b>(nrquestao).Todas().Contem(opcoes)</code>
      </pre>
