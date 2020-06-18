---
layout: post
title:  "Base Alternativa"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/base-alternativa
pasta: "funcoesv2"
mainsection: 5.27
section: 5.287
---

# Inserir Chave

*Insere uma chave e um valor na base alternativa para o cliente que está aplicando o questionário.*

- Sintaxe:
    - `BaseAlternativa().InserirChave("NOMECHAVE", "VALOR")`
- Parâmetros:
    - Chave: Nome da Chave (texto ou variável) que irá ficar associada com o valor.
    - Valor: (texto ou variável) que será associado a Chave passada.
- Exemplo 1:
    - `BaseAlternativa().InserirChave("CPF", "123.456.789-10")` 
- Exemplo 2:
    - <pre><code>
      var cpf = VL("CPF").Resposta(); //Pegando resposta da questão CPF
      BaseAlternativa().InserirChave("CPF", cpf) // Gravando a resposta da questão na Base Alternativa</code></pre>
- Exemplo 3:
    - <pre><code>
      // Não é possível ter duas chaves com o mesmo nome para um cliente.
      BaseAlternativa().InserirChave("CPF", "123.456.789-10")
      BaseAlternativa().InserirChave("CPF", "987.654.321-01") // O último valor inserido sobrescreverá o valor anterior.</code></pre>
- Exemplo 4:
    - <pre><code>
      // Um cliente pode ter várias chaves associadas a ele.
      BaseAlternativa().InserirChave("CPF", "123.456.789-10")
      BaseAlternativa().InserirChave("RG", "12.345.678-9")</code></pre>

# Contem Valor

*Verifica se na Base Alternativa do Job existe algum cliente com a chave e valor especificado.*

- Sintaxe:
    - `BaseAlternativa().ContemValor("NOMECHAVE", "VALOR")`
- Parâmetros:
    - Chave: Nome da Chave (texto ou variável) que será buscado na Base Alternativa.
    - Valor: Valor (texto ou variável) que será buscado na Base Alternativa.
- Retorno: 
    - Booleano (true/false): Se já existe um cliente no Job com a chave e valor passados retorna true, se não retorna false.
- Exemplo 1:
    - `BaseAlternativa().ContemValor("CPF", "123.456.789-10")` 
- Exemplo 2:
    - <pre><code> 
    // Exibindo uma mensagem caso já exista um cliente com a chave "CPF" e valor "123.456.789-10".
    var existeCPF = BaseAlternativa().ContemValor("CPF", "123.456.789-10")
    if (existeCPF)
    {
        Questionario().Questao("CPF").ExibirMensagem("O CPF informado já efetuou a pesquisa.")
    }</code></pre>

# Obter Valor

*Retorna o valor da chave especificada para o cliente que está aplicando o questionário.*

- Sintaxe:
    - `BaseAlternativa().ObterValor("NOMECHAVE")`
- Parâmetros:
    - Chave: Nome da Chave (texto ou variável) cujo o valor será retornado.
- Retorno: 
    - Texto: Valor associado a chave passada.
- Exemplo 1:
    - `BaseAlternativa().ObterValor("CPF")` 
- Exemplo 2:
    - <pre><code>
    BaseAlternativa().InserirChave("CPF", "123.456.789-10")
    var cpf = BaseAlternativa().ObterValor("CPF") // Armazenará na variável o valor da chave "CPF".</code></pre>

