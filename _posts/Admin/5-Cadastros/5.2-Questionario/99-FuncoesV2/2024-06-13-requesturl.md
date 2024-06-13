---
layout: post
title:  "RequestURL"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/cadastros/questionario/funcoes-fastscript/requesturl
pasta: "funcoesv2"
mainsection: 5.27
section: 5.271
---

# RequestURL
*Função para executar solicitações para urls com ou sem parametros/retorno*

- Sintaxe:
    - `RequestURL("URL")`
- Parâmetros:
    - URL: Texto/váriável do link de destino.
- Exemplo 1: 
    - `RequestURL("https://jsonplaceholder.typicode.com/posts")`
- Exemplo 2:
    - <pre>
      <code>var url: (pode ser o retorno de uma função ou estático)
      RequestURL(url)</code>
      </pre>

# Parametros (opcional)
*Função usada para fornecer informações adicionais no corpo da requisição ou na querystring (junto com a url)*

- Sintaxe:
    - `RequestURL("URL").Parametros("MÉTODO",["CHAVE=VALOR",...])`
- Parâmetros:
    - MÉTODO: Verbo HTTP usados para executar aguma ação na requisição. (opcional)
    - Podem ser: 
    - POST (Normalmente usado para gravar, registrar dados)
    - GET (Normalmente usado para obter informações)
    - PUT (Usado para atualização)
    - DELETE (Usado para deletar informações)
- Exemplo 1: 
    - POST: `RequestURL("https://jsonplaceholder.typicode.com/posts").Parametros("POST", ["CodClienteCawi=000000"])`
    - PUT: `RequestURL("https://jsonplaceholder.typicode.com/posts").Parametros("PUT", ["CodClienteCawi=000000"])`
    - DELETE: `RequestURL("https://jsonplaceholder.typicode.com/posts/1").Parametros("DELETE")`
    - GET: `RequestURL("https://jsonplaceholder.typicode.com/posts/1") Ex: o verbo GET pode ser usado passando apenas o link + /1 no caso especifico para recuperar o id 1.

# Retorno (opcional)
*Função usada para fornecer informações de retorno, o valor ao qual o campo se refere.*

- Sintaxe:
    - `.Retorno(["CHAVE"])`
- Parâmetros:
    - CHAVE: campo referente ao que é retornado quando executada a solicitação. Pode ser digitado ou variável.
- Exemplo 1:
    - `.Retorno(["nome"])`

# Exemplos de uso

- `RequestURL("https://jsonplaceholder.typicode.com/posts/1")`
- `RequestURL("https://jsonplaceholder.typicode.com/posts").Parametros("POST",["CodClienteCawi=000000"]).Retorno(["id"])`
- `RequestURL("https://jsonplaceholder.typicode.com/posts").Parametros("POST").Retorno(["Id"])`
- `RequestURL("https://jsonplaceholder.typicode.com/posts").Parametros(["chave=123456"]).Retorno(["id"])`
- `RequestURL("https://jsonplaceholder.typicode.com/posts").Retorno(["id"])`
- `RequestURL("https://jsonplaceholder.typicode.com/posts").Parametros("POST",["id=1000"])`