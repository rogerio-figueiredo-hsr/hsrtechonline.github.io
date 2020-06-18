---
layout: post
title:  "Troca Contato"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoes/trocar-contato
pasta: "funcoes"
mainsection: 5.26
section: 5.2648
---	
# $FUNCAO_EXECUTA_ACAO (TROCACONTATO;VALOR)
*Esta função está deprecada, utilizar **<a href="/fastQuestAdmin/funcoesv2/trocaContato">Trocar Contato</a>***

*Atualiza o nome do contato na listagem. Valor: novo nome*
- Parametros: 
    - ACAO: **TROCACONTATO**
    - VALOR: novo nome do contato
- Exemplo:
    - **$FUNCAO_EXECUTA_ACAO(TROCACONTATO;Fulano de Tal)**
- Resultado:
    - Atuliza na tabela de cliente o nome do contato, gerando inclusive log de troca de nome

OU

## $FUNCAO_TROCA_CONTATO

- Exemplo:
    - $FUNCAO_TROCA_CONTATO(Fulano de Tal)
