---
layout: post
title:  "Status (Grava/Força)"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/status
pasta: "funcoesv2"
---
# Força status
*Atualiza o status do cliente em memória, ou seja, o status não é efetivado*

- Sintaxe:
    - `Cliente().ForcaStatus(“CODIGOSTATUS”)`
- Parâmetros:
    - CODIGOSTATUS: Código do status (Texto entre aspas duplas) ou variável (sem aspas)
- Exemplo 1: 
    - `Cliente().ForcaStatus(“102”)`
- Exemplo 2:
    - <pre>
      <code>var codigostatus: (pode ser o retorno de uma função ou estático)
      Questionario().ForcaStatus(codigostatus)</code>
      </pre>


# Grava status
*Grava na tabela o status do cliente, ou seja, o status é efetivado e não necessita passar pelo encerramento*

- Sintaxe:
    - `Cliente().GravaStatus(“CODIGOSTATUS”)`
- Parâmetros:
    - CODIGOSTATUS: Código do status (Texto entre aspas duplas) ou variável (sem aspas)
- Exemplo 1: 
    - `Cliente().GravaStatus(“102”)`
- Exemplo 2:
    - <pre>
      <code>var codigostatus: (pode ser o retorno de uma função ou estático)
      Questionario().GravaStatus(codigostatus)</code>
      </pre>
