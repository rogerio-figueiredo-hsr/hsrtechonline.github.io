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
  - Retorna a descrição das opções declaradas na função "Descrição" retornadas da funçao **"Todas()"**
    - `<b>RM</b>("NRQUESTAO").Todas().Travar(OPCOES)`
  - Retorna a descrição das opções declaradas na função "Descrição" retornadas da funçao **"Selecionadas()"**
    - `<b>RM</b>("NRQUESTAO").<b>Selecionadas()</b>.Travar(OPCOES)`
  - Retorna a descrição das opções declaradas na função "Descrição" retornadas da funçao **"NaoSelecionadas()"**
    - `<b>RM</b>("NRQUESTAO").NaoSelecionadas().Travar(OPCOES)`
- Questao Única **(RU)**
    - Retorna a descrição das opções declaradas na função "Descrição" retornadas da funçao **"Todas()"**
      - `<b>RU</b>("NRQUESTAO").Todas().Travar(OPCOES)`
    - Retorna a opção declarada na função "Descrição" retornada da funçao **"Selecionada()"**
      - `<b>RU</b>("NRQUESTAO").<b>Selecionada()</b>.Travar(OPCOES)`
    - Retorna a descrição das opções declaradas na função "Descrição" retornadas da funçao **"NaoSelecionadas()"**
      - `<b>RU</b>("NRQUESTAO").NaoSelecionadas().Travar(OPCOES)`
  
- Parâmetros:
  - NRQUESTAO: Código da Questão (Texto entre aspas duplas) ou variável (sem aspas)
  - OPCOES: Códigos da opções numéricos entre colchetes
- Exemplo 1:
  - `<b>RM</b>("Q1").Todas().Descricao([1])`
  - `<b>RU</b>("Q1").Todas().Descricao([1])`
- Exemplo 2:
    - <pre>
      <code>var opcoes = (pode ser o retorno de uma função ou estático)
      var nrquestao = (pode ser o retorno de uma função ou estático)
      <b>RM</b>(nrquestao).Todas().Descricao(opções) ou <b>RU</b>(nrquestao).Todas().Descricao(opções)</code>
      </pre>

	  
