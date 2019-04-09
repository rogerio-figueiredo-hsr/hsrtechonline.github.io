---
layout: post
title:  "Exibir Mensagem"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoes/exibir-mensagem
pasta: "funcoes"
---
# $FUNCAO_EXECUTA_ACAO (MENSAGEM;VALOR)
*Esta função está deprecada, utilizar **<a href="/fastQuestAdmin/funcoesv2/exibirMensagem">Exibir Mensagem</a>***

Abre uma mensagem de validação na página do questionário, a mensagem aparece depois de clicar no botão prosseguir e não permitirá que o questionário avance para a próxima página

- Parâmetros: 
    - ACAO: MENSAGEM
    - VALOR: Texto que irá aparecer na tela para orientação do respondente
- Exemplo:
    - **$FUNCAO_EXECUTA_ACAO(MENSAGEM;Valor inválido, tente novamente)**
- Resultado:
    - Ao clicar no botão prosseguir a mensagem "Valor inválido, tente novamente" será exibida para o agente respondente com o intuito de orientá-lo à preencher o questionário corretamente

OU

## $FUNCAO_EXIBIR_MENSAGEM (MENSAGEM)
*Esta função está deprecada, utilizar **<a href="/fastQuestAdmin/funcoesv2/exibirMensagem">Exibir Mensagem</a>***

- Parametro:
    - MENSAGEM: Texto que irá aparecer na tela para orientação do respondente
- Exemplo:
    - **$FUNCAO_EXIBIR_MENSAGEM(Valor inválido, tente novamente)**
- Resultado:
    - Ao clicar no botão prosseguir a mensagem "Valor inválido, tente novamente" será exibida para o agente respondente com o intuito de orientá-lo à preencher o questionário corretamente
