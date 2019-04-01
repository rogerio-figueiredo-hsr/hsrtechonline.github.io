---
layout: post
title:  "Troca Telefone"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/trocaTelefone
pasta: "funcoesv2"
---
# Troca Telefone
*Atualiza um número de telefone na listagem. TELEFONE é o nr. de telefone novo e posição é qual posição do telefone será atualizada, a posição varia de 1 a 5*

- Sintaxe:
    - `Cliente().TrocaTelefone(“DDDTELEFONE”,POSICAO)`
- Parâmetros:
    - DDDTELEFONE: DDD + Telefone (Texto entre aspas duplas) ou variável (sem aspas)
    - POSICAO: posição (1 a 5) numérico
- Exemplo 1:
    - `Cliente().TrocaTelefone(“11999999999”,1)`
- Exemplo 2:
    - <pre>
      <code>var telefone = (pode ser o retorno de uma função ou estático)
      Cliente().TrocaTelefone(telefone, 1)</code>
      </pre>
