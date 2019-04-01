---
layout: post
title:  "Troca Contato"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/trocaContato
pasta: "funcoesv2"
---
# Troca Contato
*Atualiza o nome do contato na listagem.*

- Sintaxe:
    - `Cliente().TrocaContato(“NOMECONTATO”)`
- Parâmetros:
    - NOMECONTATO: Nome do Contato (Texto entre aspas duplas) ou variável (sem aspas)
- Exemplo 1:
    - `Cliente().TrocaStatus(“João da Silva”)`
- Exemplo 2:
    - <pre>
      <code>var contato: (pode ser o retorno de uma função ou estático)
      Cliente().TrocaStatus(contato)</code>
      </pre>
