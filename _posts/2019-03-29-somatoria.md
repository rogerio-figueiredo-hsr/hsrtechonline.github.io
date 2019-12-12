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

# Valores
*Retorna os valores das opções selecionadas*

- Sintaxe
  - `SM(NRQUESTAO).Selecionadas().Valores()`

- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas

- Exemplos:
  - `SM(“SM”).Selecionadas().Valores()`

# Funções de Ordenação
*Desc Asc*

# Descendente (Desc)
*Ordena na Descendente opcoes/valores/descricao*

- Sintaxe
  - `SM(NRQUESTAO).Desc(PARAMETROS).Opcoes()`
  - `SM(NRQUESTAO).Desc(PARAMETROS).Max().Opcao()`
  - `SM(NRQUESTAO).Desc(PARAMETROS).Max().Valor()`
  - `SM(NRQUESTAO).Desc(PARAMETROS).Max().Descricao()`
  - `SM(NRQUESTAO).Desc(PARAMETROS).Min().Opcao()`
  - `SM(NRQUESTAO).Desc(PARAMETROS).Min().Valor()`
  - `SM(NRQUESTAO).Desc(PARAMETROS).Min().Descricao()`
  - `SM(NRQUESTAO).Desc(PARAMETROS).Min().Valores()`

- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas
  - **(Opcional)** PARAMETROS: Informar em parâmetros o(s) número(s) da quantidade de opções ou uma variável

- Exemplos:
  - `SM(“SM”).Desc(5).Opcoes()`
  - `SM(“SM”).Desc().Min().Valor()`

# Ascendente (Asc)

- Sintaxe
  - `SM(NRQUESTAO).Asc(PARAMETROS).Opcoes()`
  - `SM(NRQUESTAO).Asc(PARAMETROS).Max().Opcao()`
  - `SM(NRQUESTAO).Asc(PARAMETROS).Max().Valor()`
  - `SM(NRQUESTAO).Asc(PARAMETROS).Max().Descricao()`
  - `SM(NRQUESTAO).Asc(PARAMETROS).Min().Opcao()`
  - `SM(NRQUESTAO).Asc(PARAMETROS).Min().Valor()`
  - `SM(NRQUESTAO).Asc(PARAMETROS).Min().Descricao()`
  - `SM(NRQUESTAO).Asc(PARAMETROS).Min().Valores()`

- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas
  - **(Opcional)** PARAMETROS: Informar em parâmetros o(s) número(s) da quantidade de opções ou uma variável

- Exemplos:
  - `SM(“SM”).Asc(5).Opcoes()`
  - `SM(“SM”).Asc().Min().Valor()`

# ParaCada

- Sintaxe
  - `SM(NRQUESTAO).Selecionadas().ParaCada(op){ }`
  - `SM(NRQUESTAO).NaoSelecionadas().ParaCada(op){ }`
  - `SM(NRQUESTAO).Todas().ParaCada(op){ }`

- Parâmetros:
  - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas

- Exemplos:
  - `SM(“SM”).Selecionadas().ParaCada(op) { ***sentença*** }`

  
# Funções Comparadoras
*Maior, MaiorIgual, Menor, MenorIgual e Entre*
*Retorna as opções, valores ou descrição conforme o comparador informado*

- Sintaxe
  - `SM(NRQUESTAO).Selecionadas().Maior(PARAMETROS1).Travar(PARAMETROS2)`
  - `SM(NRQUESTAO).Selecionadas().Maior(PARAMETROS1).Ocultar(PARAMETROS2)`
  - `SM(NRQUESTAO).Selecionadas().Maior(PARAMETROS1).Opcoes(PARAMETROS2)`
  - `SM(NRQUESTAO).Selecionadas().Maior(PARAMETROS1).Valores()`
  - `SM(NRQUESTAO).Selecionadas().Maior(PARAMETROS1).ParaCada()`
  - `SM(NRQUESTAO).Selecionadas().Maior(PARAMETROS1).Contar()`
  - `SM(NRQUESTAO).Selecionadas().Maior(PARAMETROS1).Descricao(PARAMETROS2)`
***Obs.: É a mesma sintaxe das funções ***MaiorIgual, Menor, MenorIgual***

  - `SM(NRQUESTAO).Selecionadas().Entre(PARAMETRO_INICIAL, PARAMETRO_FINAL).Travar(PARAMETROS2)`
  - `SM(NRQUESTAO).Selecionadas().Entre(PARAMETRO_INICIAL, PARAMETRO_FINAL).Ocultar(PARAMETROS2)`
  - `SM(NRQUESTAO).Selecionadas().Entre(PARAMETRO_INICIAL, PARAMETRO_FINAL).Opcoes(PARAMETROS2)`
  - `SM(NRQUESTAO).Selecionadas().Entre(PARAMETRO_INICIAL, PARAMETRO_FINAL).Valores()`
  - `SM(NRQUESTAO).Selecionadas().Entre(PARAMETRO_INICIAL, PARAMETRO_FINAL).ParaCada()`
  - `SM(NRQUESTAO).Selecionadas().Entre(PARAMETRO_INICIAL, PARAMETRO_FINAL).Contar()`
  - `SM(NRQUESTAO).Selecionadas().Entre(PARAMETRO_INICIAL, PARAMETRO_FINAL).Descricao(PARAMETROS2)`

- Parâmetros:
   - NRQUESTAO: Código da questão (Texto entre aspas duplas) ou variável sem aspas.
   - PARAMETROS1: Informar em parâmetros um número inteiro ou decimal com “.”.
   - **(Opcional)** PARAMETROS2: Informar em parâmetros um número inteiro ou decimal com “.” Ou variável.
   - PARAMETRO_INICIAL/PARAMETRO_FINAL: Número inteiro, decimal com “.” ou variável.
