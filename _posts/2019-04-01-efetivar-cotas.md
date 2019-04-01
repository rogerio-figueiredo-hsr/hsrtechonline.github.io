---
layout: post
title:  "Efetivar Cotas"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/efetivarCotas
pasta: "funcoesv2"
---

# Efetivar Cotas
*Força a efetivação da cota através da retirada da mesma de “Em andamento” para inserção dela na tabela de “entrevista realizada”*

- Sintaxe:
  - `Cotas([COTAS]).EfetivarCotas()`
- Parâmetros:
  - **(Opcional)** COTAS: Lista de códigos de cotas (entre aspas duplas e separados por vírgula
  - Obs.: COTAS não informadas, representa que não filtrará as cotas retornadas para efetivação das mesmas
- Exemplo 1:
  - `Cotas().EfetivarCotas()`
  - `Cotas(["C1","C2"]).EfetivarCotas()`
- Exemplo 2:
  - <pre>
    <code>var cotas = (pode ser o retorno de uma função ou estático)
    Cotas(cotas).EfetivarCotas()</code>
    </pre>
