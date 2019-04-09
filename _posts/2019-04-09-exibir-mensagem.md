---
layout: post
title:  "Exibir Mensagem"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/exibirMensagem
pasta: "funcoesv2"
---	

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
    Questionario().Questao(<b>nrQuestao</>).ExibirMensagem(<b>msg</b>)</code>
    </pre>
- Resultado:
  - As questões declaradas ganharão uma borda vermelha
