---
layout: post
title:  "Permissão de Usuário"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/usuario/permissao-usuario
pasta: "Usuarios"
mainsection: 2
section: 2.2
---
# Adicionando permissão ao job

Após realizar o cadastro de um usuário temos que dar acesso ao job no qual ele trabalhará, caso o contrário ele não conseguirá entrar no job.

Sob o menu de Gestão de usuários está localizado o submenu de "Permissão ao Job", clique nele.
![Menu permissão ao job]({{ "/assets/img/usuario-cadastro-menu-permissao.png" | prepend: site.baseurl }})

---- 

## Permissão por usuário

Nesta tela você selecionará um usuário, e verá todos os jobs que ele tem acesso, também poderá conceder acesso para ele em outros jobs.

### Selecionando o usuário

1. Clique em "Selecione o usuário", e todos os usuários do sistema serão listado.
![Selecionando usuários]({{ "/assets/img/usuario-permissao-select-usuario.png" | prepend: site.baseurl }})

2. Você pode utilizar a caixa de texto para buscar um usuário, pelo nome, login ou cpf. Após encontra-lo basta selecionar ele.
![Buscando usuários]({{ "/assets/img/usuario-permissao-procurando-usuario.png" | prepend: site.baseurl }})

3. Após selecionar o usuário todos os jobs do sistema serão listados, porém primeiramente será listado com a cor de fundo verde os jobs que ele já possui acesso, e por último com fundo branco os que ele não possui acesso.
![Lista de jobs do usuário]({{ "/assets/img/usuario-permissao-jobs-listados.png" | prepend: site.baseurl }})

4. Para adicionar ou remover acesso de um job basta clicar em cima dele.

5. Após definir os acessos, basta clicar no botão "Gravar".
![Botão gravar]({{ "/assets/img/usuario-permissao-botao-gravar.png" | prepend: site.baseurl }})

### Buscando por um job

1. Para buscar por um job basta clicar no ícone <i class="fa fa-search" style="color: #ff892a!important"></i>.
![Icone para buscar os jobs]({{ "/assets/img/usuario-permissao-botao-busca-job.png" | prepend: site.baseurl }})

2. Após clicar no ícone abrirá a seguinte janela:  
![Janela para buscar jobs]({{ "/assets/img/usuario-permissao-janela-busca-job.png" | prepend: site.baseurl }})

3. Selecione o campo onde será buscado o valor:
![Campos que podem ser utilizados na busca]({{ "/assets/img/usuario-permissao-campos-busca-job.png" | prepend: site.baseurl }})

4. Selecione o filtro que deseja aplicar na busca: 
![Filtros que podem ser utilizados na busca]({{ "/assets/img/usuario-permissao-filtros-busca-job.png" | prepend: site.baseurl }})

As opções de filtro que temos disponíveis são:

- Igual: Procurará por jobs onde o campo selecionado seja identico ao valor passado.
- Diferente: Procurará por jobs onde o campo selecionado seja diferente do valor passado.
- Inicia com: Procurará por jobs onde o campo selecionado inicie-se com o valor passado.
- Não inicia com: Procurará por jobs onde o campo selecionado não inicie-se com o valor passado.
- Termina com: Procurará por jobs onde o campo selecionado termina com o valor passado.
- Não termina com: Procurará por jobs onde o campo selecionado não termina com o valor passado.
- Contém: Procurará por jobs onde o campo selecionado contenha parte do valor passado.
- Não contém: Procurará por jobs onde o campo selecionado não contenha parte do valor passado.

{:start="8"}
5. Após isso preencha o campo de busca:
![Campo buscar preenchido]({{ "/assets/img/usuario-permissao-busca-job-preenchido.png" | prepend: site.baseurl }})

6. Clique no botão procurar:
![Botão procurar]({{ "/assets/img/usuario-permissao-busca-job-botao-procurar.png" | prepend: site.baseurl }})

7. Como pode ver o filtro será aplicado e será exibido na tela somente os jobs que satisfazem as condições da busca:
![Jobs filtrados]({{ "/assets/img/usuario-permissao-filtros-job-aplicado.png" | prepend: site.baseurl }})

----

## Permissão por job

Para casos onde é necessário conceder vários acessos a um determinado job recomendamos utilizar a [Permissão por job](/fastQuestAdmin/cadastros/permissao-por-job).