---
layout: post
title:  "Limpar Cotas"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/limparCotas
pasta: "funcoesv2"
---

# Limpar
*Apagar as cotas do cliente da tabela de entrevista em andamento. Todas ou informando uma lista.*

- Sintaxe:
  - `Cotas([COTAS]).Limpar()`
- Parâmetros:
  - **(Opcional)** COTAS: Lista de códigos de cotas (entre aspas duplas e separados por vírgula
  - Obs.: COTAS não informadas, representa que não filtrará as cotas retornadas para serem excluídas
- Exemplo 1:
  - `Cotas().Limpar()`
  - `Cotas(["C1","C2"]).Limpar()`
- Exemplo 2:
  - <pre>
    <code>var cotas = (pode ser o retorno de uma função ou estático)
    Cotas(cotas).Limpar()</code>
    </pre>
