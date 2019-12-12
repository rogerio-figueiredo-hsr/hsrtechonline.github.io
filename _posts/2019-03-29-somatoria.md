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

# Travar
*Trava as opções selecionadas*

- Sintaxe
  - `SM("NRQUESTAO").Selecionadas().Travar(PARAMETROS)`
  - `SM("NRQUESTAO").NaoSelecionadas().Travar(PARAMETROS)`
  - `SM("NRQUESTAO").Todas().Travar(PARAMETROS)`

- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas
  - **(Opcional)** PARAMETROS: Informar em parâmetros o(s) número(s) da(s) opção(ões) desejadas (sequência numérica entre [], número de     uma opção ou uma variável)
  
- Exemplos:
  - `SM("SM").Selecionadas().Travar([1,2,3])`
  - `SM("SM").Selecionadas().Travar(1)`
  - `SM("SM").Selecionadas().Travar()`  
  
# Ocultar
*Oculta as opções selecionadas*

- Sintaxe
  - `SM("NRQUESTAO").Selecionadas().Ocultar(PARAMETROS)`
  - `SM("NRQUESTAO").NaoSelecionadas().Ocultar(PARAMETROS)`
  - `SM("NRQUESTAO").Todas().Ocultar(PARAMETROS)`

- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas
  - **(Opcional)** PARAMETROS: Informar em parâmetros o(s) número(s) da(s) opção(ões) desejadas (sequência numérica entre [], número de     uma opção ou uma variável)
  
- Exemplos:
  - `SM("SM").Selecionadas().Ocultar([1,2,3])`
  - `SM("SM").Selecionadas().Ocultar(1)`
  - `SM("SM").Selecionadas().Ocultar()`
  
# Opcoes
*Retorna as opções selecionadas*

- Sintaxe
  - `SM(“NRQUESTAO”).Selecionadas().Opcoes(PARAMETROS)`
  - `SM("NRQUESTAO").NaoSelecionadas().Opcoes(PARAMETROS)`
  - `SM("NRQUESTAO").Todas().Opcoes(PARAMETROS)`
  
- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas
  - **(Opcional)** PARAMETROS: Informar em parâmetros o(s) número(s) da(s) opção(ões) desejadas (sequência numérica entre [], número de     uma opção ou uma variável)  
  
- Exemplos:
  - `SM("SM").Selecionadas().Opcoes([1,2,3])`
  - `SM("SM").Selecionadas().Opcoes(1)`    
  - `SM("SM").Selecionadas().Opcoes()`      

# Contar
*Retorna a quantidade de opções da questão selecionada*

- Sintaxe
  - `SM(“NRQUESTAO”).Selecionadas().Contar()`
  - `SM("NRQUESTAO").NaoSelecionadas().Contar()`
  - `SM("NRQUESTAO").Todas().Contar()`
  
- Exemplo 1:
  - `SM("SM").Selecionadas().Contar()`
  
# Descricao
*Retorna a descrição das opções selecionadas*

- Sintaxe
  - `SM(“NRQUESTAO”).Selecionadas().Descricao(PARAMETROS)`
  - `SM("NRQUESTAO").NaoSelecionadas().Contar(PARAMETROS)`
  - `SM("NRQUESTAO").Todas().Contar(PARAMETROS)`
  
- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas
  - **(Opcional)** PARAMETROS: Informar em parâmetros o(s) número(s) da(s) opção(ões) desejadas (sequência numérica entre [], número de     uma opção ou uma variável)
  
- Exemplos:
  - `SM("SM").Selecionadas().Descricao([1,2,3])`
  - `SM("SM").Selecionadas().Descricao(1)`    
  - `SM("SM").Selecionadas().Descricao()`
  
# Funções Comparadoras
*Maior, MaiorIgual, Menor, MenorIgual e Entre*
*Retorna as opções, valores ou descrição conforme o comparador informado*

# Funções de Ordenação
*Desc Asc*

# Descendente (Desc)

  - Sintaxe
  - `SM(NRQUESTAO)`
  
# Ascendente (Asc)

  - Sintaxe  

