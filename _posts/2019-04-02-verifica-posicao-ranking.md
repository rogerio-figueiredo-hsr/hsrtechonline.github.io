---
layout: post
title:  "Verifica Posicao Ranking"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/verificaPosicaoRanking
pasta: "funcoesv2"
---

# Verificar Posição Ranking
*Retorna verdadeiro se a posição informada corresponde a uma das opções do ranking informada no filtro*

- Sintaxe:
  - `RNK("NRQUESTAO").VerificarPosicao([FILTRO],POSICAO)`
- Parâmetros:
  - NRQUESTAO = Código da questão
  - FILTRO = Lista de opções do ranking (sequência numérica)
  - POSICAO = numérico inteiro
- Exemplo 1:
  - <pre>
    <code>Ranking: 5|4|1|3|2
    RNK(“Ranq”).VerificarPosicao([1,2,3], 1)</code>
    </pre>
- Exemplo 2:    
  - <pre>
    <code>var nrquestao = (pode ser o retorno de uma função ou estático)
    RNK(nrquestao).VerificarPosicao([1,2,3], 1)</code>
    </pre>
- Retorno: verdadeiro
