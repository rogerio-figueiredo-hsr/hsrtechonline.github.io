---
layout: post
title:  "Rodízio de Blocos"
projeto: "fastQuestAdminDocTec"
permalink: /fastQuestAdminDocTec/questionario/rodizio-blocos
pasta: "questionario"
---
# Rodízio de Blocos
---
Além do rodizio de páginas [ver documentação]({{ "/fastQuestAdminDocTec/questionario/questao-dinamica" | prepend: site.baseurl }}), A ordem em que as páginas não apresentadas podem ser rodiziadas por blocos, existem duas possibilidades do rodiziar por blocos:
* Somente rodiziar os blocos entre si, neste casos a ordem de apresentação dos blocos se alterna, porem a orde das páginas dentro do bloco permanece stática.  

* Rodizar blocos e páginas, neste caso além de alternar a ordem de apresentação dos blocos as páginas dentro dos blocos também terão oderm aleatória.  

## Cadastro
---

Para criar um rodízio de blocos siga os seguintes passos:  
1. clique com o botão direito na arvore de questões no nível do questionário
2. vá até a opção novo
3. clique em container, conforme imagem abaixo:

![Imagem de apoio 1]({{ "/assets/img/RodizioBlocos-01.png" | prepend: site.baseurl }})

Após essa ação teremos

![Imagem de apoio 1]({{ "/assets/img/RodizioBlocos-02.png" | prepend: site.baseurl }})

> O container é um agrupador de blocos e os blocos são agrupadores de páginas  

A criação dos containers e blocos são aramazenadas na tabela tblPaginaQuestao para poderem ser renderizadas na arvore de questionário. Porém, a ferramenta de coleta está preparada para ignorar essas páginas.
Na tabela os dados dessa estrutura ficam gravados conforme abaixo:  

select CodPaginaQuestao,Ordem,flagMostrar,CodAgrupamentoBloco,codGrupoBloco,codContainerGrupo from tblPaginaQuestao where CodQuestionario = 363  

![Imagem de apoio 1]({{ "/assets/img/RodizioBlocos-03.png" | prepend: site.baseurl }})  

> Note que as páginas 6 e 7 são respectivamente o Container e o bloco.  
  O bloco recebe os codigos:
  * CodAgrupamentoBloco = 1
  * CodGrupoBloco = 1 
  * CodContainerGrupo = 1  

O CodAgrupamentoBloco indica que existe um rodizio de blocos, e portanto quando a ferramenta de coleta encontrar uma página que tem CodAgrupamentoBloco = 1 irá criar em uma tabela auxiliar "tblOrdemBloco" uma nova ordenão para todas as páginas do mesmo CodContainerGrupo e CodGrupoBloco.  

Além da tblPaginaQuestão o container e o bloco são referenciados em outras duas tabelas tblContainerGrupo e tblGrupoBloco. Sendo que para o exemplo assim temos então:

select * from tblContainerGrupo where CodQuestionario = 363  

![Imagem de apoio 1]({{ "/assets/img/RodizioBlocos-04.png" | prepend: site.baseurl }})  


select * from tblGrupoBloco where CodQuestionario = 363  

![Imagem de apoio 1]({{ "/assets/img/RodizioBlocos-05.png" | prepend: site.baseurl }})  

Agora, no exemplo abaixo temos no mesmo questionário 2 containers e alguns blocos em cada container, e as tabelas ficam conforme abaixo:  

![Imagem de apoio 1]({{ "/assets/img/RodizioBlocos-06.png" | prepend: site.baseurl }})  

select CodPaginaQuestao,Ordem,flagMostrar,CodAgrupamentoBloco,codGrupoBloco,codContainerGrupo from tblPaginaQuestao where CodQuestionario = 363 order by ordem

![Imagem de apoio 1]({{ "/assets/img/RodizioBlocos-07.png" | prepend: site.baseurl }})  

Verifique que das páginas 6 a 21 são os blocos e páginas do container 1.  

E das páginas 8 a 26 são os blocos e páginas do container 2.  

**Obs. as páginas estão ordenadas por ordem de apresentação**  

E as tabelas de Container e bloco ficam conforme abaixo:  

select * from tblContainerGrupo where CodQuestionario = 363
select * from tblGrupoBloco where CodQuestionario = 363  

![Imagem de apoio 1]({{ "/assets/img/RodizioBlocos-07.png" | prepend: site.baseurl }})  



## Rodízio de páginas dentro do rodízio de blocos
---
Para fazer com que as páginas dentro do rodízio de blocos sejam rodiziadas deve se utilizar a opção de agrupamento de página igual ao demostrado no documento de [rodízio de páginas]({{ "/fastQuestAdminDocTec/questionario/questao-dinamica" | prepend: site.baseurl }}), observado na imagem abaixo:  

![Imagem de apoio 1]({{ "/assets/img/RodizioBlocos-09.png" | prepend: site.baseurl }})  

Note que as páginas do bloco que tem rodízio de página também recebem um código de agrupamento de página

![Imagem de apoio 1]({{ "/assets/img/RodizioBlocos-10.png" | prepend: site.baseurl }})  

Porém, diferente de seu irmão "Rodizio de páginas" a tabela que servirá de base para a ordenação rodiziada continua sendo a tblOrdemBloco como veremos a seguir.

## Navegação das páginas com Rodízio de Blocos
---

Na ferramenta de coleta ao acessar uma página que tem o CodAgrupamentoBloco = 1, todas as páginas do container são criadas na tblOrdemBloco, as páginas serão paresentadas no coleta conforme a ordem descrita na coluna Ordem, onde neste caso é possível observar na imagem a coluna codGrupoBloco (penultima coluna) que serão primeiramente exibidas as páginas do Bloco 2, depois do bloco 3 e por fim do 1 

![Imagem de apoio 1]({{ "/assets/img/RodizioBlocos-11.png" | prepend: site.baseurl }})  

## Conclusão
---
* A lógica de aplicação do rodízio de blocos é semelhante ao rodizio de páginas, proém, tem seu cadastramento facilitado através de containers e blocos visuais.
* As páginas exibidas também contém uma coluna flagQuestãoMostrou
* Ao retornar no questionário para uma página fora do rodízio de blocos e depois avançar novamente uma nova ordença das páginas será criada na tblOrdemBloco, sendo que a anterior será removida.
