---
layout: post
title:  "Buscando por usuários cadastrados"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/usuario/gestao-usuario/buscando-usuarios
pasta: "GestaoUsuarios"
mainsection: 2.1
section: 2.12
---
# Buscando por usuários cadastrados

1. Para buscar um usuário clique no ícone <i class="fa fa-search" style="color: #ff892a!important"></i>.
![Icone para buscar os registros]({{ "/assets/img/usuario-cadastro-procurar-registros.png" | prepend: site.baseurl }})

2. Após clicar no ícone abrirá a seguinte janela:  
![Janela para buscar usuários]({{ "/assets/img/usuario-cadastro-modal-buscar.png" | prepend: site.baseurl }})

3. Selecione o campo onde será buscado o valor:
![Campos que podem ser utilizados na busca]({{ "/assets/img/usuario-cadastro-campos-busca.png" | prepend: site.baseurl }})

4. Selecione o filtro que deseja aplicar na busca: 
![Filtros que podem ser utilizados na busca]({{ "/assets/img/usuario-cadastro-filtros-busca.png" | prepend: site.baseurl }})

As opções de filtro que temos disponíveis são:

- Igual: Procurará por usuários onde o campo selecionado seja identico ao valor passado.
- Diferente: Procurará por usuários onde o campo selecionado seja diferente do valor passado.
- Inicia com: Procurará por usuários onde o campo selecionado inicie-se com o valor passado.
- Não inicia com: Procurará por usuários onde o campo selecionado não inicie-se com o valor passado.
- Termina com: Procurará por usuários onde o campo selecionado termina com o valor passado.
- Não termina com: Procurará por usuários onde o campo selecionado não termina com o valor passado.
- Contém: Procurará por usuários onde o campo selecionado contenha parte do valor passado.
- Não contém: Procurará por usuários onde o campo selecionado não contenha parte do valor passado.

{:start="5"}
5. Após isso preencha o campo de busca:
![Campo de busca preenchido]({{ "/assets/img/usuario-cadastro-janela-busca-preenchida.png" | prepend: site.baseurl }})

6. Clique no botão procurar:
![Botão procurar]({{ "/assets/img/usuario-cadastro-botao-procurar.png" | prepend: site.baseurl }})


7. Como pode ver o filtro será aplicado e será exibido na tela somente quem satisfaz as condições da busca:
![Filtro de usuário aplicado]({{ "/assets/img/usuario-cadastro-filtrado.png" | prepend: site.baseurl }})

---

## Aplicando mais de um filtro na busca

Caso deseje aplicar mais de um filtro para realizar uma busca mais complexa.

1. Clique no botão com ícone de +. Para cada vez que clicar neste ícone um novo filtro aparecerá em baixo do anterior.
![Adicionar novo filtro]({{ "/assets/img/usuario-cadastro-add-criterio.png" | prepend: site.baseurl }})

2. Após isto basta preencher os dados dos filtros e clicar em "Procurar".
![Multiplos filtros preenchidos]({{ "/assets/img/usuario-cadastro-multiplos-filtros.png" | prepend: site.baseurl }})

3. Como podem ver o filtro para os dois campos que especifiquei foram aplicados.
![Multiplos filtros aplicados]({{ "/assets/img/usuario-cadastro-filtrado-multiplos.png" | prepend: site.baseurl }})

Caso deseje remover os filtros que foram aplicados na lista de usuários basta clicar no botão "Resetar"
![Botão resetar filtros]({{ "/assets/img/usuario-cadastro-resetar-filtro.png" | prepend: site.baseurl }})


