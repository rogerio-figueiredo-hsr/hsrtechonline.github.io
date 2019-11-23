---
layout: post
title:  "Rodízios de Página"
projeto: "fastQuestAdminDocTec"
permalink: /fastQuestAdminDocTec/questionario/rodizio-pagina
pasta: "questionario"
---
# Rodízio de Páginas
---
No cadastro de questionário é possível agrupar as páginas de forma que as páginas serão apresentadas em uma ordem aleatória.

Por exemplo, se você cadastrar na ordem:   
Páginas 1,2 e 3 essas páginas sempre serão apresentadas no coleta exatamente nesta mesma ordem conforme imagens abaixo:  
![Imagem ordem das paginas]({{"/assets/img/RodizioPaginas_01.png"| prepend: site.baseurl}})

No banco de dados essas paginas são armazenadas na tblPaginaQuestão com as seguintes ordens:

![Imagem ordem das paginas]({{"/assets/img/RodizioPaginas_02.png"| prepend: site.baseurl}})

Na ferramenta de coleta a navegação ocorre sempre da ordem mais baixa para ordem mais alta, sendo assim as páginas serão sempre apresentadas na ordem páginas: 1,2,3  

## Agrupar as páginas com o objetivo de randomizar (Rodiziar)  
---

É possivel Randomizar a ordem em que as páginas são apresentadas na ferramenta de coleta.  
Essa randomização ocorre em tempo de aplicação do questionário, ou seja, acontece no momento em que se entra em uma página agrupada.  
Para agrupar as páginas é necessário prencher no cadastro da página o campo Agrup. Página (Agrupamento de página)  

![Imagem ordem das paginas]({{"/assets/img/RodizioPaginas_03.png"| prepend: site.baseurl}})

Essa informação fica armazenada na tblPaginaQuestao na coluna  CodAgrupamentoPagina

![Imagem ordem das paginas]({{"/assets/img/RodizioPaginas_04.png"| prepend: site.baseurl}})  

Na ferramenta de coleta durante a navegação das páginas é que ocorre a interpretação desse dado.  
Quando é encontrada uma página que tenha um número maior que zero nessa coluna, todas as páginas que tem o mesmo número são agrupadas juntas e criado em uma tabela auxiliar de nome: "tblRodizioCliente" uma ordenação que substitua a ordenação da tblPaginaquestão  

select CodQuestionario,CodPaginaQuestao,Ordem,CodAgrupamentoPagina from tblPaginaQuestao where CodQuestionario = 363 order by ordem  

select * from tblClienteRodizio where CodCliente = 2813951 order by ordem  

![Imagem ordem das paginas]({{"/assets/img/RodizioPaginas_05.png"| prepend: site.baseurl}})  

Na imagem acima é possível verifica que:  
* Na tblPaginaQuestão a ordem permanece inalterada, sendo que temos as pagias 2,3 e 4 em sequência
* Na tblClienteRodizio para o codCliente 2813951, foi criada uma outra odem com as páginas: 3, 2 e 4, que seráo exibidas exatamente nessa ordem.  

>Observe também o FlaQuestaoMostrou essa flag indica as páginas que ja foram apresentadas para o entrevistado ou entrevistador.

## Conclusão
---

Portanto é possível concluir que a rotina que localiza a próxima página a ser exibida no questinário faz um "left join" com a tblClienteRodizio.  
> Sendo assim se a página encontrada para ser aplicada possui um valor maior que zero na coluna CodAgrupamento, será necessário buscar todas as páginas desse questionário com CodAgrupamento "igual" colocar todas essas páginas na tblClienteRodizio com seus respectivos agrupamentos e pegar a primeira página dessa tabela como  sendo a próxima a ser aplicada, as demais páginas desse mesmo agrupamento serão exibidas uma a uma de acordo com FalgQuestaoMostrou.  

A procedure que retorna a próxima página a ser exibida e tem toda essa regra de negócio é: pr_RetornaPaginaQuestaoProxima  

Essa procedure é camada toda vez que o entrevistado clica no botrão prosseguir da ferramenta de coleta
