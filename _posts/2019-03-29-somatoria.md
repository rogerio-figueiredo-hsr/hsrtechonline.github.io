---
layout: post
title:  "Somatória"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/somatoria
pasta: "funcoesv2"
---

# Somar
*Retorna a soma dos valores das opções informadas.*

- Sintaxe: 
  - `SM(“NRQUESTAO”).Selecionadas().Somar([OPCOES])}`
- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas
  - OPCOES: Sequência numérica informado com o numero das opções da questão.
- Exemplo 1: 
  - `SM(“Soma”).Selecionadas().SomarOpcoes([1,2,3])`
- Exemplo 2: 
  - <pre>
    <code>var nrquestao = (pode ser o retorno de uma função ou estático)
    var opcoes = (pode ser o retorno de uma função ou estático)
    SM(nrquestao).Selecionadas().SomarOpcoes(opcoes)</code>
    </pre>
- Retorno: 
  - A soma dos valores

# Max (Opções, Valor, Descrição)
*Retorna o maior valor entre as opções respondidas*

- Sintaxe: 
  - `SM(“NRQUESTAO”).Selecionadas().Max([OPCOES]).Opcao()`
  - `SM(“NRQUESTAO”).Selecionadas().Max([OPCOES]).Valor()`
  - `SM(“NRQUESTAO”).Selecionadas().Max([OPCOES]).Descricao()`  
- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas
  - OPCOES: (OPCIONAL) Opcoes entre colchetes e separados por vírgula
- Exemplo 1:
  - `1@10|2@20|3@30|4@0`
  - `SM(“Soma”).Selecionadas().Max().Valor()`
  - `SM(“Soma”).Selecionadas().Max([1,2]).Valor()`
- Exemplo 2:
  - `1@10|2@20|3@30|4@0`
  - `SM(“Soma”).Selecionadas().Max().Opcao()`  
- Exemplo 3:
  - <pre>
    <code>var nrquestao = (pode ser o retorno de uma função ou estático)
    SM(nrquestao).Selecionadas().Max()</code>
    </pre>
- Retorno:
  - Ex: 1
    - 30
    - 20 (filtrado)
  - Ex: 2
    - 2    
  - Ex: 3
    - 30

# Min (Opções, Valor, Descrição)
*Retorna o menor valor entre as opções respondidas*

- Sintaxe: 
  - `SM(“NRQUESTAO”).Selecionadas().Min().Opcao()`
  - `SM(“NRQUESTAO”).Selecionadas().Min().Valor()`
  - `SM(“NRQUESTAO”).Selecionadas().Min().Descricao()` 
- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas
- Exemplo 1:
  - `1@10|2@20|3@30|4@0`
  - `SM(“Soma”).selecionadas().Min().Valor()`
  - `SM(“Soma”).Selecionadas().Min([2,4]).Valor()`
- Exemplo 2:
  - `1@10|2@20|3@30|4@0`
  - `SM(“Soma”).Selecionadas().Min().Opcao()`  
- Exemplo 3:  
  - <pre>
    <code>var nrquestao: (pode ser o retorno de uma função ou estático)
    SM(nrquestao).Selecionadas().Min()</code>
    </pre>
- Retorno:
  - Ex: 1
    - 30
    - 20 (filtrado)
  - Ex: 2
    - 2    
  - Ex: 3
    - 30


# Selecionadas
*Retorna as opções selecionadas*

- Sintaxe: 
  - Trava as opções declaradas na função “Travar” 
    - `SM(“NRQUESTAO”).Selecionadas().Travar(OPCOES)`
  - Oculta as opções declaradas na função “Ocultar”
    - `SM(“NRQUESTAO”).Selecionadas().Ocultar(OPCOES)`
  - Verifica se os códigos das “Opções” declaradas na função “Contem”, existem no retorno das opções selecionadas. Caso sim, retorna         verdadeiro, senão falso
    - `SM(“NRQUESTAO”).Selecionadas().Contem(OPCOES)`
  - Retorna as opções declaradas na função “Opcoes”
    - `SM(“NRQUESTAO”).Selecionadas().Opcoes(OPCOES)`
  - Itera sobre todas as opções retornadas da função Selecionadas. O parâmetro “op” representa cada opção retornada de “Selecionadas”
    - <pre>
      <code>SM(“NRQUESTAO”).Selecionadas().ParaCada(op){ 
      “Sentença para ser executada ”
      }</code>
      </pre> 
  - Retorna quantidade de opções não selecionadas
    - `SM(“NRQUESTAO”).Selecionadas().Contar()`
  - Retorna a descrição das opções declaradas na função “Descricao”
    - `SM(“NRQUESTAO”).Selecionadas().Descricao(OPCOES)`
- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas
  - **(Opcional)** PARAMETROS: Informar em parâmetros o(s) número(s) da(s) opção(ões) desejadas (sequência numérica entre [], número de     uma opção ou uma variável)
- Exemplo 1:
  - `SM("SM").Selecionadas().Travar([1,2,3])`
- Exemplo 2:
  - <pre>
    <code>Var nrquestao = (pode ser o retorno de uma função ou estático)
    var opcoes = (pode ser o retorno de uma função ou estático)
    SM(nrquestao).Selecionadas().Travar([opções])</code>
    </pre>

# Não Selecionadas
*Retorna as opções que não foram selecionadas*

- Sintaxe: 
  - Trava as opções declaradas na função “Travar” 
    - `SM(“NRQUESTAO”).NaoSelecionadas().Travar(OPCOES)`
  - Oculta as opções declaradas na função “Ocultar”
    - `SM(“NRQUESTAO”).NaoSelecionadas().Ocultar(OPCOES)`
  - Verifica se os códigos das “Opções” declaradas na função “Contem”, existem no retorno das opções selecionadas. Caso sim, retorna         verdadeiro, senão falso
    - `SM(“NRQUESTAO”).NaoSelecionadas().Contem(OPCOES)`
  - Retorna as opções declaradas na função “Opcoes”
    - `SM(“NRQUESTAO”).NaoSelecionadas().Opcoes(OPCOES)`
  - Itera sobre todas as opções retornadas da função Selecionadas. O parâmetro “op” representa cada opção retornada de “Selecionadas”
    - <pre>
      <code>SM(“NRQUESTAO”).NaoSelecionadas().ParaCada(op){ 
      “Sentença para ser executada ”
      }</code>
      </pre>
  - Retorna quantidade de opções não selecionadas
    - `SM(“NRQUESTAO”).NaoSelecionadas().Contar()`
  - Retorna a descrição das opções declaradas na função “Descricao”
    - `SM(“NRQUESTAO”).NaoSelecionadas().Descricao(OPCOES)`
- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas
  - **(Opcional)** PARAMETROS: Informar em parâmetros o(s) número(s) da(s) opção(ões) desejadas. sequência numérica entre [], número de     uma opção ou uma variável.
- Exemplo 1:
  - `SM("SM").NaoSelecionadas().Travar([1,2,3])`
- Exemplo 2:
  - <pre>
    <code>var opcoes = (pode ser o retorno de uma função ou estático)
    var nrquestao = (pode ser o retorno de uma função ou estático)
    SM("nrquestao ").NaoSelecionadas().Travar(opcoes)</code>
    </pre>
