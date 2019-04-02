---
layout: post
title:  "Descriçao"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/descricao
pasta: "funcoesv2"
---

# Descricao()
*Retorna a descriçao das opções declaradas na função **"Descricao()"***

- Sintaxe:
- Questoes Multiplas **(RM)**
  - Retorna a descrição das opções declaradas na função "Descricao()" retornadas da funçao **"Todas()"**
    - `<b>RM</b>("NRQUESTAO").Todas().Descricao(OPCOES)`
  - Retorna a descrição das opções declaradas na função "Descricao()" retornadas da funçao **"Selecionadas()"**
    - `<b>RM</b>("NRQUESTAO").<b>Selecionadas()</b>.Descricao(OPCOES)`
  - Retorna a descrição das opções declaradas na função "Descricao()" retornadas da funçao **"NaoSelecionadas()"**
    - `<b>RM</b>("NRQUESTAO").NaoSelecionadas().Descricao(OPCOES)`
- Questao Única **(RU)**
  - Retorna a descrição das opções declaradas na função "Descricao()" retornadas da funçao **"Todas()"**
    - `<b>RU</b>("NRQUESTAO").Todas().Descricao(OPCOES)`
  - Retorna a descrição das opções declarada na função "Descricao()" retornada da funçao **"Selecionada()"**
    - `<b>RU</b>("NRQUESTAO").<b>Selecionada()</b>.Descricao(OPCOES)`
  - Retorna a descrição das opções declaradas na função "Descricao()" retornadas da funçao **"NaoSelecionadas()"**
    - `<b>RU</b>("NRQUESTAO").NaoSelecionadas().Descricao(OPCOES)`
- Ranking **(RNK)**
  - **Não Implementado**
    - Retorna a descrição das opções declaradas na função "Descricao()" retornadas da funçao **"Todas()"**
      - `<b>RNK</b>("NRQUESTAO").Todas().Descricao(OPCOES)`
  - Retorna a descrição das opções declaradas na função "Descricao()" retornadas da funçao **"Selecionadas()"**
    - `<b>RNK</b>("NRQUESTAO").<b>Selecionadas()</b>.Descricao(OPCOES)`
  - Retorna a descrição das opções declaradas na função "Descricao()" retornadas da funçao **"NaoSelecionadas()"**
    - `<b>RNK</b>("NRQUESTAO").NaoSelecionadas().Descricao(OPCOES)`
- Somatoria **(SM)**
  - **Não Implementado**
    - Retorna a descrição das opções declaradas na função "Descricao()" retornadas da funçao **"Todas()"**
      - `<b>SM</b>("NRQUESTAO").Todas().Descricao(OPCOES)`
  - Retorna a descrição da opções declaradas na função "Descricao()" retornadas da funçao **"Selecionadas()"**
    - `<b>SM</b>("NRQUESTAO").<b>Selecionadas()</b>.Descricao(OPCOES)`
  - Retorna a descrição da opções declaradas na função "Descricao()" retornadas da funçao **"NaoSelecionadas()"**
    - `<b>SM</b>("NRQUESTAO").NaoSelecionadas().Descricao(OPCOES)`
  
- Parâmetros:
  - NRQUESTAO: Código da Questão (Texto entre aspas duplas) ou variável (sem aspas)
  - OPCOES: Códigos da opções numéricos entre colchetes
- Exemplo 1:
  - `<b>RM</b>("Q1").Todas().Descricao([1])`
  - `<b>RU</b>("Q1").Todas().Descricao([1])`
  - `<b>RNK</b>("Q1").Selecionadas().Descricao([1])`
  - `<b>SM</b>("Q1").Selecionadas().Descricao([1])`
- Exemplo 2:
    - <pre>
      <code>var opcoes = (pode ser o retorno de uma função ou estático)
      var nrquestao = (pode ser o retorno de uma função ou estático)
      <b>RM</b>(nrquestao).Todas().Descricao(opções) ou <b>RU</b>(nrquestao).Todas().Descricao(opções)</code>
      </pre>

	  
