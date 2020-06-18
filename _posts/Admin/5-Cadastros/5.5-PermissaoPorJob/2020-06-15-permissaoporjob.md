---
layout: post
title:  "Permissão ao Job"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/cadastros/permissao-por-job
pasta: "Cadastros"
mainsection: 5
section: 5.5
---
# Permissão por Job

A Permissão por Job pode ser feita através do menu “Cadastros” que fica localizado dentro de um job:

![Menu permissão por job]({{ "/assets/img/cadastros-permissaoporjob-menu.png" | prepend: site.baseurl }})

Clicando no menu abrirá a tela de Permissão por Job, nela vocês terão a visão de dois grids:

![Tela permissão por job]({{ "/assets/img/cadastros-permissaoporjob-tela.png" | prepend: site.baseurl }})

 - "Usuários NÃO Associados": Neste grid será listado todos os usuários do sistema que não possuem acesso dentro desse job.
 - "Usuários Associados": "Neste grid será listado todos os usuários que possuem acesso ao job."

Ambos os grids são divididos em páginas, cada página exibirá no máximo 500 usuários:

![Paginas do grid]({{ "/assets/img/usuario-permissao-paginas.png" | prepend: site.baseurl }})

---

## Buscando usuário

Caso deseje buscar por um usuário especifico, basta utilizar a barra de busca localizada em cima de cada grid. 

1. Preencha o campo de busca com o nome, CPF ou login do usuário.
![Preenchendo campo de busca]({{ "/assets/img/cadastros-permissaoporjob-buscando.png" | prepend: site.baseurl }})

2. Clique no botão "Buscar".
![Botão buscar]({{ "/assets/img/cadastros-permissaoporjob-buscar-botao.png" | prepend: site.baseurl }})

3. Após isto, o filtro será aplicado e somente os usuários que possuam o que foi digitado será listado.
![Grid filtrado após buscar]({{ "/assets/img/cadastros-permissaoporjob-filtro-aplicado.png" | prepend: site.baseurl }})

4. Caso deseje remover o filtro basta clicar no <i class="fa fa-times"></i> ao lado do botão "Buscar". 
![Botão X]({{ "/assets/img/cadastros-permissaoporjob-buscar-botao-limpar.png" | prepend: site.baseurl }})

---

## Concedendo permissões em um job

1. Selecione no grid de "Usuários NÃO Associados" os usuários que deseja conceder acesso ao job.
![Selecionando usuário no grid de Usuários NÃO Associados]({{ "/assets/img/cadastros-permissaoporjob-concedendo-permissao.png" | prepend: site.baseurl }})

2. Clique na seta apontando para o grid de "Usuários Associados".
![Seta apontando para usuários associados]({{ "/assets/img/cadastro-permissaoporjob-seta-usuarios-associados.png" | prepend: site.baseurl }})

3. Imediatamente após clicar, os usuários que estavam selecionados estarão com acesso ao projeto, logo irão desaparecer do grid “Usuários NÃO Associados” e aparecerão no grid “Usuários Associados”.
![Usuários movidos para o grid de associados]({{ "/assets/img/cadastros-permissaoporjob-permissao-concedida.png" | prepend: site.baseurl }})

---

## Removendo permissões do job

1. Selecione no grid de "Usuários Associados" os usuários que deseja remover o acesso ao job.
![Selecionando usuário no grid de Usuários Associados]({{ "/assets/img/usuario-permissao-removendo-usuarios.png" | prepend: site.baseurl }})

2. Clique na seta apontando para o grid de "Usuários NÃO Associados".
![Seta apontando para usuários não associados]({{ "/assets/img/usuario-permissao-seta-usuariosnaoassociados.png" | prepend: site.baseurl }})

3. Após clicar imediatamente os usuários selecionados perderão o acesso ao projeto, e em consequência irão desaparecer do grid “Usuários Associados” e aparecer no grid “Usuários NÃO Associados”.
![Usuários movidos para o grid de desassociados]({{ "/assets/img/cadastro-permissaoporjob-usuarios-desassociados.png" | prepend: site.baseurl }})