---
layout: post
title:  "Somatória"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/somatoria
pasta: "funcoesv2"
---

# Somar Opções
*Retorna a soma dos valores das opções informadas.*

Sintaxe: 
SM(“NRQUESTAO”).SomarOpcoes([OPCOES])}
Parâmetros:
NRQUESTAO = Código da questão (Texto entre aspas duplas) ou variável sem aspas
OPCOES = Sequência numérica informado com o numero das opções da questão.

Ex.: 
SM(“Soma”).SomarOpcoes([1,2,3])
var nrquestao = (pode ser o retorno de uma função ou estático)
var opcoes = (pode ser o retorno de uma função ou estático)
SM(nrquestao).SomarOpcoes(opcoes)

Retorno: a soma dos valores

# Max
*Retorna o maior valor entre as opções respondidas*

Sintaxe: 
SM(“NRQUESTAO”).Max()
Parâmetros:
NRQUESTAO = Código da questão (Texto entre aspas duplas) ou variável sem aspas

Ex.: 
1@10|2@20|3@30|4@0
SM(“Soma”).Max()

Var nrquestao = (pode ser o retorno de uma função ou estático)
SM(nrquestao).Max()

Retorno: 30


# Min
*Retorna o menor valor entre as opções respondidas*

Sintaxe: 
SM(“NRQUESTAO”).Min()
Parâmetros:
NRQUESTAO = Código da questão (Texto entre aspas duplas) ou variável sem aspas

Ex.: 
1@10|2@20|3@30|4@0
SM(“Soma”).Min()

var nrquestao = (pode ser o retorno de uma função ou estático)
SM(nrquestao).Min()

Retorno: 10


# Selecionadas
*Retorna as opções selecionadas*

Sintaxe: 
Trava as opções declaradas na função “Travar” 
SM(“NRQUESTAO”).Selecionadas().Travar(OPCOES)

Oculta as opções declaradas na função “Ocultar”
SM(“NRQUESTAO”).Selecionadas().Ocultar(OPCOES)

Verifica se os códigos das “Opções” declaradas na função “Contem”, existem no retorno das opções selecionadas. Caso sim, retorna verdadeiro, senão falso
SM(“NRQUESTAO”).Selecionadas().Contem(OPCOES)

Retorna as opções declaradas na função “Opcoes”
SM(“NRQUESTAO”).Selecionadas().Opcoes(OPCOES)

Itera sobre todas as opções retornadas da função Selecionadas. O parâmetro “op” representa cada opção retornada de “Selecionadas”
SM(“NRQUESTAO”).Selecionadas().ParaCada(op){ 
“Sentença para ser executada ”
}

Retorna quantidade de opções não selecionadas
SM(“NRQUESTAO”).Selecionadas().Contar()

Retorna a descrição das opções declaradas na função “Descricao”
SM(“NRQUESTAO”).Selecionadas().Descricao(OPCOES)

Parâmetros:
NRQUESTAO = Código da questão (Texto entre aspas duplas) ou variável sem aspas
(Opcional) PARAMETROS = Informar em parâmetros o(s) número(s) da(s) opção(ões) desejadas (sequência numérica entre [], número de uma opção ou uma variável)
Ex.:
SM("SM").Selecionadas().Travar([1,2,3])

Var nrquestao = (pode ser o retorno de uma função ou estático)
var opcoes = (pode ser o retorno de uma função ou estático)
SM(nrquestao).Selecionadas().Travar([opções])


# Não Selecionadas
*Retorna as opções que não foram selecionadas*

Sintaxe: 
Trava as opções declaradas na função “Travar” 
SM(“NRQUESTAO”).NaoSelecionadas().Travar(OPCOES)

Oculta as opções declaradas na função “Ocultar”
SM(“NRQUESTAO”).NaoSelecionadas().Ocultar(OPCOES)

Verifica se os códigos das “Opções” declaradas na função “Contem”, existem no retorno das opções selecionadas. Caso sim, retorna verdadeiro, senão falso
SM(“NRQUESTAO”).NaoSelecionadas().Contem(OPCOES)

Retorna as opções declaradas na função “Opcoes”
SM(“NRQUESTAO”).NaoSelecionadas().Opcoes(OPCOES)

Itera sobre todas as opções retornadas da função Selecionadas. O parâmetro “op” representa cada opção retornada de “Selecionadas”
SM(“NRQUESTAO”).NaoSelecionadas().ParaCada(op){ 
“Sentença para ser executada ”
}

Retorna quantidade de opções não selecionadas
SM(“NRQUESTAO”).NaoSelecionadas().Contar()

Retorna a descrição das opções declaradas na função “Descricao”
SM(“NRQUESTAO”).NaoSelecionadas().Descricao(OPCOES)

Parâmetros:
NRQUESTAO = Código da questão (Texto entre aspas duplas) ou variável sem aspas
(Opcional) PARAMETROS = Informar em parâmetros o(s) número(s) da(s) opção(ões) desejadas. sequência numérica entre [], número de uma opção ou uma variável.
Ex.:
SM("SM").NaoSelecionadas().Travar([1,2,3])

var opcoes = (pode ser o retorno de uma função ou estático)
var nrquestao = (pode ser o retorno de uma função ou estático)
SM("nrquestao ").NaoSelecionadas().Travar(opcoes)