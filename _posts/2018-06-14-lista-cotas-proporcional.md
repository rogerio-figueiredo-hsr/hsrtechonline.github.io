---
layout: post
title:  "Lista de Cotas Proporcional"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoes/lista-cotas-proporcional
pasta: "funcoes"
---
# $FUNCAO_RETORNA_COTAS_PROPORCIONAL (QTDCOTAS;LISTA*)
Retorna uma lista com cotas que tem metas a serem cumpridas ordenadas pela cota menos cumprida até a cotá mais próxima de cumprir.
OBS.: Pode se também delimitar um range de cotas atráves do parametro (LISTA), que quando informado, busca a cota menos realizada dentro do range informado.
- Parametros: 
    - QTDCOTAS: número inteiro que indica a quantidade de cotas que se deseja trabalhar ordenadas da cota mais distante de ser cumprida até a cota menos cumprida
    - LISTA*: parametro opcional, deve ser uma lista de códigos de cota separados por PIPE
- Exemplo:
    - **$FUNCAO_RETORNA_COTAS_PROPORCIONAL(5)**
- Resultado:
    - C12\|C2\|C31\|C1\|C3
        - Esta função pode ser associada com a $FUNCAO_LOOP por exemplo, de modo a ocultar ou direcionar o questionário para um determinado bloco.
- Obs.:
    - Esta função retorna apenas cotas com metas ">0 " (maior que zero) cadastradas e apenas cotas ativas