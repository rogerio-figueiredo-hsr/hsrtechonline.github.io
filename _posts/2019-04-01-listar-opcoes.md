---
layout: post
title:  "Listar Opções"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/listarOpcoes
pasta: "funcoesv2"
---

# Opcoes()
*Lista as opções declaradas na função **"Opcoes()"***

- Sintaxe:
- Questoes Multiplas **(RM)**
  - Retorna a lista das opções declaradas na função "Opcoes()" retornadas da funçao **"Todas()"**
    - `<b>RM</b>("NRQUESTAO").Todas().Opcoes(OPCOES)`
  - Retorna a lista das opções declaradas na função "Opcoes()" retornadas da funçao **"Selecionadas()"**
    - `<b>RM</b>("NRQUESTAO").<b>Selecionadas()</b>.Opcoes(OPCOES)`
  - Retorna a lista das opções declaradas na função "Opcoes()" retornadas da funçao **"NaoSelecionadas()"**
    - `<b>RM</b>("NRQUESTAO").NaoSelecionadas().Opcoes(OPCOES)`
- Questao Única **(RU)**
    - Retorna a lista das opções declaradas na função "Opcoes()" retornadas da funçao **"Todas()"**
      - `<b>RU</b>("NRQUESTAO").Todas().Opcoes(OPCOES)`
    - Retorna a lista das opções declaradas na função "Opcoes()" retornadas da funçao **"NaoSelecionadas()"**
      - `<b>RU</b>("NRQUESTAO").NaoSelecionadas().Opcoes(OPCOES)`
- **Não Implementado**      
  - Ranking **(RNK)**
    - Trava as opções declaradas na função "Opcoes" retornadas da funçao **"Todas()"**
      - `<b>RNK</b>("NRQUESTAO").Todas().Opcoes(OPCOES)`
    - Trava as opções declaradas na função "Opcoes" retornadas da funçao **"Selecionadas()"**
      - `<b>RNK</b>("NRQUESTAO").<b>Selecionadas()</b>.Opcoes(OPCOES)`
    - Trava as opções declaradas na função "Opcoes" retornadas da funçao **"NaoSelecionadas()"**
      - `<b>RNK</b>("NRQUESTAO").NaoSelecionadas().Opcoes(OPCOES)`
  - Somatoria **(SM)**
    - Trava as opções declaradas na função "Opcoes" retornadas da funçao **"Todas()"**
      - `<b>SM</b>("NRQUESTAO").Todas().Opcoes(OPCOES)`
    - Trava as opções declaradas na função "Opcoes" retornadas da funçao **"Selecionadas()"**
      - `<b>SM</b>("NRQUESTAO").<b>Selecionadas()</b>.Opcoes(OPCOES)`
    - Trava as opções declaradas na função "Opcoes" retornadas da funçao **"NaoSelecionadas()"**
      - `<b>SM</b>("NRQUESTAO").NaoSelecionadas().Opcoes(OPCOES)`
- Parâmetros:
  - NRQUESTAO: Código da Questão (Texto entre aspas duplas) ou variável (sem aspas)
  - OPCOES: Códigos da opções numéricos entre colchetes
- Exemplo 1:
  - `<b>RM</b>("Q1").Todas().Opcoes([1])`
  - `<b>RU</b>("Q1").Todas().Opcoes([1])`
- Exemplo 2:
    - <pre>
      <code>var opcoes = (pode ser o retorno de uma função ou estático)
      var nrquestao = (pode ser o retorno de uma função ou estático)
      <b>RM</b>(nrquestao).Todas().Opcoes(opções) ou <b>RU</b>(nrquestao).Todas().Opcoes(opções)</code>
      </pre>
