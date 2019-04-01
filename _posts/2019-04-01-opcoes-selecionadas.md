---
layout: post
title:  "Listar Opções Selecionadas"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/opcoesSelecionadas
pasta: "funcoesv2"
---

# Selecionadas

- Sintaxe:
  - Trava as opções declaradas na função "Travar" 
    - `RM("NRQUESTAO").Selecionadas().Travar(OPCOES)`
  - Oculta as opções declaradas na função "Ocultar"
    - `RM("NRQUESTAO").Selecionadas().Ocultar(OPCOES)`
  - Verifica se os códigos das "Opções" declaradas na função "Contem", existem no retorno das opções selecionadas. Caso sim, retorna         verdadeiro, senão falso
    - `RM("NRQUESTAO").Selecionadas().Contem(OPCOES)`
  - Retorna as opções declaradas na função "Opcoes"
    - `RM("NRQUESTAO").Selecionadas().Opcoes(OPCOES)`
  - Itera sobre todas as opções retornadas da função Selecionadas. O parâmetro "op" representa cada opção retornada de "Selecionadas"
    - <pre>
      <code>RM("NRQUESTAO").Selecionadas().ParaCada(op){
      "Sentença para ser executada"
      }</code>
      </pre>
  - Retorna quantidade de opções selecionadas
    - `RM("NRQUESTAO").Selecionadas().Contar()`
  - Retorna a descrição das opções declaradas na função "Descricao"
    - `RM("NRQUESTAO").Selecionadas().Descricao(OPCOES)`
- Parâmetros:
  - NRQUESTAO: Código da Questão (Texto entre aspas duplas) ou variável (sem aspas)
  - **(Opcional)** OPCOES: Códigos da opções numéricos entre colchetes ou variável (sem aspas)
- Exemplo 1:
  - `RM("Q1").Selecionadas().Selecionadas().Travar([1,2,3]))`
    Obs.: Mesma sintaxe para as outras funções. 
- Exemplo 2:
  - <pre>
    <code>var opcoes = (pode ser o retorno de uma função ou estático)
    var nrquestao = (pode ser o retorno de uma função ou estático)
    RM(nrquestao).Selecionadas().Travar(opcoes)</code>
    </pre>
