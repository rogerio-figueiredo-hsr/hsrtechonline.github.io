---
layout: post
title:  "Para Cada (Loop)"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/paraCada
pasta: "funcoesv2"
---

# ParaCada()
*Itera sobre todas as opções retornadas da função Selecionadas. O parâmetro "op" representa cada opção retornada da funçao anterior*

- Sintaxe
  - <pre>
    <code>RM("NRQUESTAO").Selecionadas().ParaCada(op){
    "Sentença para ser executada"
    }</code>
    </pre>
  *Obs.: **ParaCada** pode ser usada por Questões múltiplas (RM) e Questão única (RU), após as seguintes funçoes: Todas(), Selecionadas ou NaoSelecionadas().*
  
- Parâmetros:
  - NRQUESTAO: Código da Questão (Texto entre aspas duplas) ou variável (sem aspas)
  - op: representa cada uma das opções retornadas da função anterior
- Exemplo:
  - <pre>
    <code>RM("Q1").Selecionadas().ParaCada(op){
      RM("Q2").Todas().Ocultar(op)
    }
    </pre>
