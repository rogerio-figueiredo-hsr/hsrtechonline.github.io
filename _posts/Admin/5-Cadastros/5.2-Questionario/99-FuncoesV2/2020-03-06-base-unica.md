---
layout: post
title:  "Base Única"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/cadastros/questionario/funcoes-fastscript/base-unica
pasta: "funcoesv2"
mainsection: 5.27
section: 5.288
---

# Valor Coluna

*Retorna o valor da coluna e cliente passados por parametro.*

- Sintaxe:
    - `BaseUnica("CPF").Coluna("NOMECOLUNA").Valor()`
- Parâmetros:
    - CPF: CPF (texto ou variável) do cliente que será buscado na Base Única.
    - NomeColuna: Nome da Coluna (texto ou variável) que será buscada na Base Única.
- Retorno: 
    - Texto: Valor associado a coluna e ao cliente.
- Exemplo 1:
    - `BaseUnica("12345678910").Coluna("RG").Valor()` 
- Exemplo 2:
    - <pre><code>
    var cpf = VL("CPF").Resposta()
    var rg = BaseUnica(cpf).Coluna("RG").Valor() // Guardará em uma variável o RG do cliente buscado na Base Única.</code></pre>

