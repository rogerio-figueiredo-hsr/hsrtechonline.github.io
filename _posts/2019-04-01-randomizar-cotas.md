---
layout: post
title:  "Randomizar Cotas"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/randomizarCotas
pasta: "funcoesv2"
---

# Randomizar Cotas
*Retorna a lista de cotas de forma randomizada.*

- Sintaxe:
  - `Cotas([COTAS]).Randomizar()`
- Parâmetros:
   - **(Opcional)** COTAS: Lista de códigos de cotas (entre aspas duplas e separados por vírgula
- Exemplo 1:
  - `Cotas().Randomizar()`
  - `Cotas(["C1","C2"]).Randomizar()`
- Exemplo 2:
  - <pre>
    <code>var cotas = (pode ser o retorno de uma função ou estático)
    Cotas(cotas).Randomizar()</code>
    </pre>
- Resultado:
  - C2\|C1
