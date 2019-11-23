---
layout: post
title:  "Questão Dinâmica"
projeto: "fastQuestAdminDocTec"
permalink: /fastQuestAdminDocTec/questionario/questao-dinamica
pasta: "questionario"
---
# Questão Dinâmica
---
A questão dinâmica permite que um conjuto de Páginas/Questões seja replicado para todas as opções cadastratadas nesta questão.  

---
# Exemplo
---
![Imagem de apoio 1]({{ "/assets/img/QuestaoDinamica1.png" | prepend: site.baseurl }})

Na imagem acima temos uma questão dinâmica "BASE_DM1" com 3 páginas associadas a ela: "Página 9, 14 e 19" note que a questão dinâmica possui  4 Opções   

Então estruturalmente a questão dinãmica gera as seguintes páginas na tabela tblPaginaQuestao:  
    * Query utilizada: select * from tblPaginaQuestao where CodQuestionario = \{Codigo do questionário\} and NrQuestaoPrincipal = '{NrQuestao dinâmica}' ORDER BY ORDEM
    * Onde o "Codigo do questionário" é o código do questionário e "NrQuestao dinâmica" é o NrQuestao da dinâmica
    * No exemplo acima tempos o seguinte resultado


| CodPaginaQuestao|flagPrincipal|flagDinamica|NrQuestaoPrincipal|OpcaoPrincipal|CodPaginaQuestaoPrincipal|
|-----------------|:-----------:|-----------:|-----------------:|-------------:|------------------------:|
|9	              |1	        |0	         |BASE_DM1	        |NULL	       |NULL                     |
|14	              |1	        |0	         |BASE_DM1	        |NULL	       |NULL                     |
|19	              |1	        |0	         |BASE_DM1	        |NULL	       |NULL                     |
|10	              |0	        |1	         |BASE_DM1	        |1	           |9	                     |
|15	              |0	        |1	         |BASE_DM1	        |1	           |14	                     |
|20	              |0	        |1	         |BASE_DM1	        |1	           |19	                     |
|11	              |0	        |1	         |BASE_DM1	        |2	           |9	                     |
|16	              |0	        |1	         |BASE_DM1	        |2	           |14	                     |
|21	              |0	        |1	         |BASE_DM1	        |2	           |19	                     |
|12	              |0	        |1	         |BASE_DM1	        |3	           |9	                     |
|17	              |0	        |1	         |BASE_DM1	        |3	           |14	                     |
|22	              |0	        |1	         |BASE_DM1	        |3	           |19	                     |
|13	              |0	        |1	         |BASE_DM1	        |4	           |9	                     |
|18	              |0	        |1	         |BASE_DM1	        |4	           |14	                     |
|23	              |0	        |1	         |BASE_DM1	        |4	           |19	                     |
  


Onde as páginas 9,14,19 são as páginas principais "flagPrincipal = 1 ", ou seja as páginas que serão replicadas para cada opção e portando não aparecem no questionário.  
Apartir da ágina 10 até a página 23 são as páginas geradas para cada opção "flagDinamica=1" onde é possível ver através da coluna OpcaoPrincipal a referencia entre a questão gerada e para qual 
opção ela se aplica, e na coluna CodPaginaQuestaoPrincipal, é possível identificar qual a página foi usada como referência para essa replicação.  

Então temos:  
páginas 10,15 e 20 são cópias da página 9,14 e 19 respectivamente aplicadas para a opção 1 da Base Dinâmica
páginas 11,16 e 21 são cópias da página 9,14 e 19 respectivamente aplicadas para a opção 2 da Base Dinâmica
páginas 12,17 e 22 são cópias da página 9,14 e 19 respectivamente aplicadas para a opção 3 da Base Dinâmica
páginas 13,18 e 23 são cópias da página 9,14 e 19 respectivamente aplicadas para a opção 4 da Base Dinâmica

![Imagem de apoio 1]({{ "/assets/img/QuestaoDinamica2.png" | prepend: site.baseurl }})