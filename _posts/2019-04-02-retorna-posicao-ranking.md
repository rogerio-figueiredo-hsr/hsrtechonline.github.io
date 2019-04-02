---
layout: post
title:  "Posição Raking"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/posicaoRanking
pasta: "funcoesv2"
---

# Posicao()
*Retorna o número do item clicado conforme posição fornecida.*

- Sintaxe: 
  - `RNK("NRQUESTAO").Posicao(POSICAO)`
  - `RNK("NRQUESTO").Posicao(POSICAO).Descricao()
- Parâmetros:
  - NRQUESTAO = Código da questão
  - POSICAO = número inteiro que quando informado, retorna apenas uma opção de acordo com a ordem solicitada.
- Exemplo 1: 
  - Ranking: 5|4|2|10|7
  - RNK("Ranq").Posicao(1)
  - RNK("Ranq").Posicao(1).Descricao()
- Exemplo 2: 
  - <pre>
    <code>var nrquestao = (pode ser o retorno de uma função ou estático)
    var pos = (pode ser o retorno de uma função ou estático)
    RNK(nrquestao).Posicao(pos)</code>
    <pre>
- Retorno: 5
  ***Obs.: Se usado com a função "Descricao()" retorna o nome da opção.***
