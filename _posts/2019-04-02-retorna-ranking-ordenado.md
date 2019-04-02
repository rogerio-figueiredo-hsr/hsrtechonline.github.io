---
layout: post
title:  "Ranking Ordenado"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/rankingOrdenado
pasta: "funcoesv2"
---

# Ascendente (Asc())
*Retorna o ranking dos itens ordenado na ascendente conforme a quantidade de itens solicitados (QTD OPCOES)*

- Sintaxe:
  - `RNK(“NRQUESTAO”).Asc(QTDOPCOES)`
- Parâmetros:
  - NRQUESTAO = Código da questão
  - (Opcional) QTDOPCOES = Quantidade de opções para serem retornadas.
- Exemplo 1:
  - <pre>
    <code>Ranking: 5|4|2|10|7
    RNK(“Ranq”).Asc(3)</code>
    </pre>
- Exemplo 2:
  - <pre>
    <code>var nrquestao = (pode ser o retorno de uma função ou estático)
    var qtdOpcoes = (pode ser o retorno de uma função ou estático)
    RNK(nrquestao).Asc(qtdOpcoes)</code>
    </pre>
- Retorno: 5\|4\|2

# Descendente (Desc())
*Retorna o ranking dos itens na descendente conforme a quantidade de itens solicitados (QTD OPCOES)*

- Sintaxe:
  - `RNK(“NRQUESTAO”).Desc(QTDOPCOES)`
- Parâmetros:
  - NRQUESTAO = Código da questão
  - (Opcional) QTDOPCOES = Quantidade de opções informadas como filtro
- Exemplo 1:
  - <pre>
    <code>Ranking: 5|4|2|10|7
    RNK(“Ranq”).Desc(3)</code>
    </pre>
- Exemplo 2:
  - <pre>
    <code>var nrquestao = (pode ser o retorno de uma função ou estático)
    var qtdOpcoes = (pode ser o retorno de uma função ou estático)
    RNK(nrquestao).Desc(qtdOpcoes)</code>
    </pre>
- Retorno: 7\|10\|2
