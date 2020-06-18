---
layout: post
title:  "Questionario"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/questionario
pasta: "funcoesv2"
mainsection: 5.27
section: 5.274
---
# Pular Página
*Indica para qual página o questionário será redirecionado.*
- Sintaxe:
    - `Questionario().Pagina(PARAMETROS)`
- Parâmetros:
    - PARAMETROS: informar o número da página, o nome da questão entre aspas ou uma variável.
- Exemplo 1:
    - `Questionario().Pagina(1)`
    - `Questionario().Pagina(“Q1”)`
- Exemplo 2:
    - <pre>
      <code>var param = (pode ser o retorno de uma função ou estático)`
      Questionario().Pagina(param)</code>
      </pre>
- Resultado:
    - Questionário será redirecionado para a página/questão fornecida  


# Próxima Página
*Pula para a próxima página*
- Sintaxe: 
    - `Questionario().ProximaPagina()`
- Exemplo:
    - `Questionario().ProximaPagina()`
- Resultado:
    - Questionário pulará para a próxima página.


# Ocultar Questão
*Oculta uma ou mais questões conforme parâmetro informado na função "Questão"*
- Sintaxe: 
    - `Questionario().Questao(QUESTOES).Ocultar()`
- Parâmetros:
    - QUESTOES: Nomes das questões entre chaves em sequência literal entre aspas duplas separados por vírgula.
- Exemplo 1:
    - `Questionario().Questao([“Q1”,”Q2”,”Q3”]).Ocultar()`
- Exemplo 2:
    - <pre>
      <code>var param = (pode ser o retorno de uma função ou estático)
      Questionario().Questao(param).Ocultar()</code>
      </pre>
- Resultado:
    - Questões informadas serão ocultadas


# Ocultar botão voltar
*Oculta o botão "Voltar"*
- Sintaxe:
    - `Questionario().OcultarVoltar()`
- Exemplo:
    - `Questionario().OcultarVoltar()`
- Resultado:
    - Botão voltar será ocultado

# Ocultar botão Prosseguir
*Oculta o botão "Prosseguir"*
- Sintaxe: 
    - `Questionario().OcultarProsseguir()`
- Exemplo:
    - `Questionario().OcultarProsseguir()`
- Resultado:
    - Botão "Prosseguir" será ocultado

# Liberar botão Voltar
*Exibe o botão "Voltar" caso esteja oculto*
- Sintaxe:
    - `Questionario().LiberaVoltar()`
- Exemplo: 
    - `Questionario().LiberaVoltar()`
- Resultado:
    - Botão "Voltar" será exibido
    
# Exibir Mensagem
*Abre uma mensagem de validação na página do questionário, a mensagem aparece depois de clicar no botão prosseguir e não permitirá que o questionário avance para a próxima página e marcará as questões para serem reavaliadas com borda vermelha*

- Sintaxe:
  - `Questionario().Questao(QUESTAO).ExibirMensagem(MENSAGEM)`
- Parâmetros:
  - QUESTAO: Questão(ões) que serão marcadas na página com borda em vermelho. Se for uma única questão, colocar entre aspas duplas, se for mais de uma colocar cada uma delas entre aspas duplas separadas por vírgula e envolvê-las com chaves, ou ainda variável sem aspas e chaves.
  - MENSAGEM: A mensagem a ser exibida entre aspas duplas ou variável.
- Exemplo 1:
  - `Questionario().Questao("Q1").ExibirMensagem("Mensagem Teste")`
  - `Questionario().Questao(["Q1","Q2"]).ExibirMensagem("Mensagem Teste")`
- Exemplo 2:
  - <pre>
    <code>var <b>nrQuestao</b> = (estático ou o retorno de outra função)
    var <b>msg</b> = (estático ou o retorno de outra função)
    Questionario().Questao(<b>nrQuestao</b>).ExibirMensagem(<b>msg</b>)</code>
    </pre>
- Resultado:
  - As questões declaradas ganharão uma borda vermelha    
    

