---
layout: post
title:  "Manipular Sequências"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/manipularSequencias
pasta: "funcoesv2"
---

# Contem
*Verifica se uma condição é atendida, dada uma sequência de numeros fixos ou o retorno de uma função armazenada em uma variável*

- Sintaxe:
  - `(PARAMETRO1).Contem(PARAMETRO2)`
- Parâmetros:
  - PARAMETRO1: Sequências de números separados por vírgula entre parênteses. Cada bloco de sequências, separados por vírgula     e         entre colchetes, número inteiro ou variável. Ex.: ([1,2],[3,4]). Obs.: é mais usado para receber uma dados não conhecidos               armazenados em variáveis.
  - PARAMETRO2: Número inteiro ou variável que representa o valor a ser avaliado com a sequência numérica informada.
- Exemplos:
  - `([1-20],[21,23,25]).Contem(10)`
  - `var opcoes = RM("Teste").Selecionadas().Opcoes(); (opcoes).Contem(10)`
  
# ParaCada
*Itera sobre cada numero dentro do manipulador*

- Sintaxe:
  - `(PARAMETRO1).ParaCada(PARAMETRO2){...}`
- Parâmetros:
  - PARAMETRO: Sequências de números separados por vírgula entre parênteses. Cada bloco de sequências, separados por vírgula e     entre colchetes ou variável. Ex.: ([1,2],[3,4]). Obs.: é mais usado para receber uma dados não conhecidos armazenados em variáveis.
  - PARAMETRO2: Este é um operador (definir qualquer nome) que será controlado automaticamente dentro do laço nas iterações.
- Exemplos:
  - `([1-20],[21,23,25]).ParaCada(op){ ... }`
  - `var opcoes = RM("Teste").Selecionadas().Opcoes(); (opcoes).ParaCada(op) { ... }`

# Randomizar
*Randomiza a sequênicia informada*

- Sintaxe:
  - `(PARAMETRO1).Randomizar(PARAMETRO2)`
- Parâmetros:
  - PARAMETRO1: Sequências de números separados por vírgula entre parênteses. Cada bloco de sequências, separados por                       vírgula e entre colchetes ou variavel. Ex.: ([1,2],[3,4]). Obs.: é mais usado para receber uma dados não conhecidos armazenados em       variáveis
  - PARAMETRO2: Variável ou número inteiro que parametriza a quantidade de números a ser randomizados.
- Exemplos:
  - `([1-20],[21,23,25]).Randomizar(5)`
  - `var opcoes = RM("Teste").Selecionadas().Opcoes(); (opcoes).Randomizar(10) { ... }`
