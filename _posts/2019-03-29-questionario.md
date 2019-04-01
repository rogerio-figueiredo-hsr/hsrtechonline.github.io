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
    - `Questionario().Pagina(PARAMETROS)`
- Parâmetros:
    - PARAMETROS: informar o número da página, o nome da questão entre aspas ou uma variável.
- Exemplo 1:
    - `Questionario().Pagina(1)`
    - `Questionario().Pagina(“Q1”)`
- Exemplo 2:
    - <pre>
      <code>var param = (pode ser o retorno de uma função ou estático)`
      Questionario().Pagina(param)</code>
      </pre>
- Resultado:
    - Questionário será redirecionado para a página/questão fornecida  


# Próxima Página
*Pula para a próxima página*
- Sintaxe: 
    - `Questionario().ProximaPagina()`
- Exemplo:
    - `Questionario().ProximaPagina()`
- Resultado:
    - Questionário pulará para a próxima página.


# Ocultar Questão
*Oculta uma ou mais questões conforme parâmetro informado na função "Questão"*
- Sintaxe: 
    - `Questionario().Questao(QUESTOES).Ocultar()`
- Parâmetros:
    - QUESTOES: Nomes das questões entre chaves em sequência literal entre aspas duplas separados por vírgula.
- Exemplo 1:
    - `Questionario().Questao([“Q1”,”Q2”,”Q3”]).Ocultar()`
- Exemplo 2:
    - <pre>
      <code>var param = (pode ser o retorno de uma função ou estático)
      Questionario().Questao(param).Ocultar()</code>
      </pre>
- Resultado:
    - Questões informadas serão ocultadas


# Ocultar botão voltar
*Oculta o botão "Voltar"*
- Sintaxe:
    - `Questionario().OcultarVoltar()`
- Exemplo:
    - `Questionario().OcultarVoltar()`
- Resultado:
    - Botão voltar será ocultado

# Ocultar botão Prosseguir
*Oculta o botão "Prosseguir"*
- Sintaxe: 
    - `Questionario().OcultarProsseguir()`
- Exemplo:
    - `Questionario().OcultarProsseguir()`
- Resultado:
    - Botão "Prosseguir" será ocultado

# Liberar botão Voltar
*Exibe o botão "Voltar" caso esteja oculto*
- Sintaxe:
    - `Questionario().LiberaVoltar()`
- Exemplo: 
    - `Questionario().LiberaVoltar()`
- Resultado:
    - Botão "Voltar" será exibido    
    

