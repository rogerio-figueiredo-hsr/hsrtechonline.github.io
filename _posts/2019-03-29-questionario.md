---
layout: post
title:  "Questionario"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/questionario
pasta: "funcoesv2"
---
# Pular Página
*Indica para qual página o questionário será redirecionado.*
- Sintaxe:
    - **Questionario().Pagina(PARAMETROS)**
- Parâmetros:
    - NUMERO: informar o número da página.
    - NOME DA QUESTAO: informar o nome da questão.
- Exemplo:
    - **Questionario().Pagina(1)**
    - **Questionario().Pagina(“Q1”)**
- Resultado:
    - Questionário será redirecionado para a página/questão fornecida  

# Próxima Página
*Pula para a próxima página*
- Sintaxe: Questionario().ProximaPagina()
- Exemplo:
    - **Questionario().ProximaPagina()**
- Resultado:
    - Questionário pulará para a próxima página.

# Ocultar Questão
*Oculta a questao conforme parâmetro informado na função "Questão"*
- Sintaxe: 
    - **Questionario().Questao(QUESTOES).Ocultar()**
- Parâmetros:
    - QUESTOES: Nomes das questões entre chaves em sequência literal entre aspas duplas separados por vírgula.

Ex.:
Questionario().Questao([“Q1”,”Q2”,”Q3”]).Ocultar()

# Ocultar botão voltar
**
Sintaxe: Questionario().OcultarVoltar()
Ex.:
Questionario().OcultarVoltar()

# Ocultar botão Prosseguir
**
Sintaxe: Questionario().OcultarProsseguir()
Ex.:
Questionario().OcultarProsseguir()


# Liberar botão Voltar
**
- Sintaxe:
    - Questionario().LiberaVoltar()

Ex.: Questionario().LiberaVoltar()
