  ---
layout: post
title:  "Listar Opções Não Selecionadas"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/opcoesNaoSelecionadas
pasta: "funcoesv2"
---

# Não Selecionadas

- Sintaxe:
  - Trava as opções declaradas na função "Travar"
    - `RM("NRQUESTAO").NaoSelecionadas().Travar(OPCOES)`
  - Oculta as opções declaradas na função "Ocultar"
    - `RM("NRQUESTAO").NaoSelecionadas().Ocultar(OPCOES)`
  - Verifica se os códigos das "Opções" declaradas na função "Contem", existem no retorno das opções selecionadas. Caso sim, retorna         verdadeiro, senão falso
    - `RM("NRQUESTAO").NaoSelecionadas().Contem(OPCOES)`
  - Retorna as opções declaradas na função "Opcoes"
    - `RM("NRQUESTAO").NaoSelecionadas().Opcoes(OPCOES)`
  - Itera sobre todas as opções retornadas da função Selecionadas. O parâmetro "op" representa cada opção retornada de "Selecionadas"
    - <pre>
      <code>RM("NRQUESTAO").NaoSelecionadas().ParaCada(op){
      "Sentença para ser executada"
      }</code>
      </pre>
  - Retorna quantidade de opções não selecionadas
    - `RM("NRQUESTAO").NaoSelecionadas().Contar()`
  - Retorna a descrição das opções declaradas na função 'Descricao"
    - `RM("NRQUESTAO").NaoSelecionadas().Descricao(OPCOES)`
- Parâmetros:
    - NRQUESTAO: Código da Questão (Texto entre aspas duplas) ou variável (sem aspas)
    - **(Opcional)** OPCOES: Códigos da opções numéricos entre colchetes ou variável (sem aspas)
- Exemplo 1:
  - `RM("Q1").NaoSelecionadas().Travar([1,2,3])`
  Obs.: Mesma sintaxe para as outras funções.
- Exemplo 2:  
  - <pre>
    <code>var opcoes = (pode ser o retorno de uma função ou estático)
    var nrquestao = (pode ser o retorno de uma função ou estático)
    RM(nrquestao).NaoSelecionadas().Travar(opções)</code>
    <pre>
