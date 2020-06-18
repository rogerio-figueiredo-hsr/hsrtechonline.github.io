---
layout: post
title:  "Cancelamentos"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/entrevista/devolver-entrevistas
pasta: "Entrevista"
mainsection: 7
section: 7.2
---
# Entrevistas canceladas

Para uma entrevista ser cancelada ela precisa ter sido em algum momento realizada. 

Aqui é possível realizar a visualização das entrevistas canceladas, sendo que existem duas
possibilidades:

---

## Devolver entrevistas por IDs

Devolvemos entrevistas canceladas para o status de realizada (102) através do código dos clientes.

1. Adicione os IDs dos clientes que deseja devolver no campo "Lista de clientes";
![Lista de clientes]({{ "/assets/img/entrevistas-cancelamento-lista-ids.png" | prepend: site.baseurl }})

2. Clique em "Alterar";
![Botão alterar]({{ "/assets/img/entrevistas-cancelamento-botao-alterar.png" | prepend: site.baseurl }})

3. Uma janela se abrirá pedindo para confirmar se realmente deseja devolver a entrevista para realizada;
![Janela confirmação]({{ "/assets/img/entrevistas-cancelamento-confirmacao.png" | prepend: site.baseurl }})

4. Caso esteja certo disso clique em "OK" e imediatamente os IDs voltarão para o status realizado;
![Botão OK]({{ "/assets/img/entrevistas-cancelamento-botao-confirmacao.png" | prepend: site.baseurl }})

---

## Devolver entrevistas por status

Na aba por status podemos consultar todas as entrevistas que foram canceladas e se
necessário retorná-las para realizadas.

1. Clique na aba status.
![Aba status]({{ "/assets/img/entrevistas-cancelamento-aba-status.png" | prepend: site.baseurl }})

2. Selecione o status que deseja visualizar os clientes. Aqui será listado todos os status que encerram, veja mais sobre [Status](/fastQuestAdmin/cadastros/status).
![Lista de status]({{ "/assets/img/entrevistas-cancelamento-selecione-status.png" | prepend: site.baseurl }})

3. Clique em "Pesquisar".
![Botão Pesquisas]({{ "/assets/img/entrevistas-cancelamento-botao-pesquisar.png" | prepend: site.baseurl }})

4. Todos os clientes no status selecionado serão listados no grid logo abaixo.
![Lista de clientes cancelados]({{ "/assets/img/entrevistas-cancelamento-lista-cancelados.png" | prepend: site.baseurl }})

- **Código:** Código do cliente.
- **Situação atual:** Status atual do cliente.
- **Cancelado por:** Usuário do sistema que alterou o status do cliente para cancelado.
- **Data cancelamento:** Data que o cliente foi cancelado.
- **Entrevistador:** Quem entrevistou o cliente.
- **Data Entrevista:** Data que o cliente foi entrevistado.
- **Duração:** A duração da coleta de respostas em segundos.

{:start="5"}
5. Selecione os clientes que deseja devolver para o status de realizado. 
![Cliente selecionados]({{ "/assets/img/entrevistas-cancelamento-selecionando-devolvidos.png" | prepend: site.baseurl }})

6. Clique em "Alterar";
![Botão alterar]({{ "/assets/img/entrevistas-cancelamento-botao-alterar.png" | prepend: site.baseurl }})

7. Uma janela se abrirá pedindo para confirmar se realmente deseja devolver a entrevista para realizada;
![Janela confirmação]({{ "/assets/img/entrevistas-cancelamento-confirmacao.png" | prepend: site.baseurl }})

8. Caso esteja certo disso clique em "OK" e imediatamente os clientes selecionados voltarão para o status realizado;
![Botão OK]({{ "/assets/img/entrevistas-cancelamento-botao-confirmacao.png" | prepend: site.baseurl }})