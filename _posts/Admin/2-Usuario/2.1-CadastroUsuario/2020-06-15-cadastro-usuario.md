---
layout: post
title:  "Cadastrar um novo usuário"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/usuario/gestao-usuario/cadastro-usuario
pasta: "GestaoUsuarios"
mainsection: 2.1
section: 2.11
---
# Cadastrar um novo usuário

1. Para cadastrar um novo usuário clique no ícone <i class="fa fa-plus-circle" style="color: #a069c3!important"></i>.

![Incluindo novo registro]({{ "/assets/img/cadastro-de-usuario-02.png" | prepend: site.baseurl }})

{:start="2"}
2. Preencha todos campos do formulário com dados válidos:  

![Preenchendo os dados do usuário]({{ "/assets/img/usuario-cadastro-incluir-novo.png" | prepend: site.baseurl }})

- Nome: O nome completo do usuário que está sendo cadastrado.
- CPF: O CPF do usuário a ser cadastrado.
- Login: O login que será utilizado para acessar o sistema.
- Senha: Tem acesso restrito de acordo com o que for determinado
- E-mail: E-mail que será utilizado em caso de recuperação de senha.
- Perfil: É o que definirá as permissões que o usuário terá no sistema.
- Id da PA: É o login que o usuário utiliza para entrar no PABX. 
    **Atenção: Caso este campo não esteja preenchido corretamente o entrevistador será incapaz de utilizar algumas funcionalidades do PABX.**
- Trocar senha: Se marcado fará com que o usuário tenha que trocar a senha ao efetuar o login.

Em Perfil teremos as opções:

- Admin: Tem acesso a todas áreas do sistema.
- Diretoria: Tem acesso restrito de acordo com o que for determinado.
- Gerencia: Tem acesso restrito de acordo com o que for determinado.
- Client Service: Tem acesso restrito de acordo com o que for determinado.
- Entrevistador: Não tem acesso ao site administrativo.

Em Idioma teremos as opções:

- Português.
- Espanhol.
- Inglês.

{:start="3"}
3. Após o preenchimento de todos os dados clique no botão "Enviar" e o usuário será cadastrado.

![Botão para enviar os dados do formulário de usuário]({{ "/assets/img/usuario-cadastro-botao-enviar.png" | prepend: site.baseurl }})
