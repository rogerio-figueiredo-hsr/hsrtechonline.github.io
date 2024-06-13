---
layout: post
title:  "RequestURL"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/cadastros/questionario/funcoes-fastscript/base-geral
pasta: "funcoesv2"
mainsection: 5.27
section: 5.271
---

# ObterValorBase
*Função para executar em bancos de dados*

- Sintaxe:
    - `BaseGeral("BANCO+TABELA").ObterValorBase("FILTRO_COLUNA","FILTRO_VALOR","COLUNA_RETORNO")`
- Parâmetros:
    - BANCO+TABELA: Texto/váriável do banco de dados + tabela.
    - FILTRO_COLUNA: Texto/váriável com o nome da coluna onde será consultada.
    - FILTRO_VALOR: Texto/váriável com o valor da coluna onde será consultada.
    - COLUNA_RETORNO: Texto/váriável com o nome da coluna que retornará o valor.
- Exemplo 1: 
    - `BaseGeral("base_cep_dbo.Job_1234").ObterValorBase("numero","123456","data")`