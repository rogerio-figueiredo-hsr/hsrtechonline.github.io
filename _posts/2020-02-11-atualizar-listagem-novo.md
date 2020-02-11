---
layout: post
title:  "Atualizar Listagem Novo"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/listagem/atualizar-listagem-novo
pasta: "Listagem"
---

# Atulizar Listagem

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

{:start="6"}
6. Faça as alterações necessárias no arquivo CSV gerado, mas mantenha a primeira coluna "CodCliente" intacta, é através desta coluna que o FastQuest identificará quais registros deverão ser atualizados
![Imagem de apoio 4]({{ "/assets/img/lista-atualizacao.png" | prepend: site.baseurl }})

{:start="7"}
7. Para fazer a atualização dos registros:
<div class="row" markdown="1">
<div class="6u 12u$(small)" markdown="1">
*A primeira linha do arquivo deve conter o nome das colunas que serão importadas
*A primeira coluna deve conter o campo "CodCliente" que foi exportado anteriormente
*Deixe apenas um cliente por linha
*A separação das colunas no arquivo CSV pode ser por ";" ou "|"
*Selecione o arquivo para atualização
*Defina qual é a separação das colunas
*Marque a opção "Atualizar listagem" e clique em "Processar"
</div>
<div class="6u 12u$(small)" markdown="1">
    ![Imagem de apoio 4]({{ "/assets/img/atualizacao-listagem.png" | prepend: site.baseurl }})
</div>
</dib>