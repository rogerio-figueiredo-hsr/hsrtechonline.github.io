---
layout: post
title:  "Atualizar Listagem Novo"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/listagem/atualizar-listagem-novo
pasta: "Listagem"
---

# Atualizar Listagem

<div class="row" markdown="1">
<div class="6u 12u$(small)" markdown="1">
1. Selecione o projeto na página inicial;

2. Após o projeto estar selecionado e ter redirecionado para a página do mesmo, clique em "Gestão de dados";

3. Irá abrir um SubMenu, ache a opção "Listagem" e clique;
</div>
<div class="6u 12u$(small)" markdown="1">
![Imagem de apoio 1]({{ "/assets/img/adicionar-listagem-01.png" | prepend: site.baseurl }})
</div>                               
</div>

{:start="4"}
4. Sigas as intruções para fazer uma importação 
![Imagem de apoio 2]({{ "/assets/img/instrucoes-listagem-atualizar.png" | prepend: site.baseurl }})

{:start="5"}
5. Faça a exportacao do arquivo que você deseja atualizar
![Imagem de apoio 3]({{ "/assets/img/exportar-listagem-novo-01.png" | prepend: site.baseurl }})

<div class="row" markdown="1">
<div class="6u 12u$(small)" markdown="1">
{:start="6"}
6. Faça as alterações necessárias no arquivo CSV gerado, mas mantenha a primeira coluna "CodCliente" intacta, é através desta coluna que o FastQuest identificará quais registros deverão ser atualizados
</div>

<div class="6u 12u$(small)" markdown="1">
![Imagem de apoio 4]({{ "/assets/img/lista-atualizacao.png" | prepend: site.baseurl }})
</div>
</div>

{:start="7"}
7. Para fazer a atualização dos registros:
<div class="row" markdown="1">
<div class="6u 12u$(small)" markdown="1">
* A primeira linha do arquivo deve conter o nome das colunas que serão importadas
* A primeira coluna deve conter o campo "CodCliente" que foi exportado anteriormente
* Deixe apenas um cliente por linha
* A separação das colunas no arquivo CSV pode ser por ";" ou "\|".
* Selecione o arquivo para atualização
* Defina qual é a separação das colunas
* Marque a opção "Atualizar listagem" e clique em "Processar"
</div>
<div class="6u 12u$(small)" markdown="1">
![Imagem de apoio 5]({{ "/assets/img/atualizacao-listagem-novo.png" | prepend: site.baseurl }})
</div>
</div>

{:start="8"}
8. Após clicar no botão "Processar", será adicionado um novo item na lista "Lista de processamentos". Assim que o arquivo for processado será enviada uma mensagem através do sistema de mensagens (sino)
![Imagem de apoio 6]({{ "/assets/img/lista-processamento.png" | prepend: site.baseurl }})

{:start="9"}
9.  Caso queira cancelar o processamento clique no icone da "Lixeira"
(Não é possível cancelar o processo após o inicio)
![Imagem de apoio 7]({{ "/assets/img/atualizacao-listagem-novo-02.png" | prepend: site.baseurl }})

---

## Se não existir todos os campos da listagem

<div class="row" markdown="1">
<div class="6u 12u$(small)" markdown="1">
1. Clique em "Gerenciar campos adicionais";
</div>
<div class="6u 12u$(small)" markdown="1">
![Imagem de apoio 8]({{ "/assets/img/instrucoes-listagem-02.png" | prepend: site.baseurl }})
</div>                               
</div>


<div class="row" markdown="1">
<div class="6u 12u$(small)" markdown="1">
{:start="2"}
2. Clique em "Adicionar Campo";
</div>
<div class="6u 12u$(small)" markdown="1">
![Imagem de apoio 9]({{ "/assets/img/instrucoes-listagem-03.png" | prepend: site.baseurl }})
</div>
</div>

<div class="row" markdown="1">
<div class="6u 12u$(small)" markdown="1">
{:start="3"}
3. Adicione uma "Descrição";

4. Adicione o "Nome da Coluna" existente na listagem a ser importada;

5. "CodTipoDado" é o tipo dos dados existentes na coluna;

6. Selecione "Aceitar nulo" se o campo não for obrigatório;

7. Clique em "Enviar";
</div>
<div class="6u 12u$(small)" markdown="1">
![Imagem de apoio 10]({{ "/assets/img/adicionar-listagem-04.png" | prepend: site.baseurl }})
</div>
</div>

<div class="row" markdown="1">
<div class="6u 12u$(small)" markdown="1">
{:start="8"}
8. Caso queira adicionar mais de um campo de um só vez, clique em "Como importar campos adicionais"
</div>
<div class="6u 12u$(small)" markdown="1">
![Imagem de apoio 9]({{ "/assets/img/instrucoes-listagem-04.png" | prepend: site.baseurl }})
</div>
</div>
