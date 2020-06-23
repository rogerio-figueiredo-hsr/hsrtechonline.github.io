---
layout: post
title:  "Encerrando cliente"
projeto: "fastQuestColeta"
permalink: /fastQuestColeta/questionario/encerrando-cliente
pasta: ""
mainsection: 3
section: 3.5
---

# Encerrando um cliente

1. Clique no botão "Encerrar" ou pressione a tecla "F6".
![Botão encerrar]({{ "/assets/img/coleta/botao-encerrar.png" | prepend: site.baseurl }})

2. A janela de encerramento se abrirá:
![Janela agendamento]({{ "/assets/img/coleta/janela-agendamento.png" | prepend: site.baseurl }}){:width="700px"}

3. Clique na aba "Encerramento".
![Aba encerramento]({{ "/assets/img/coleta/aba-encerramento.png" | prepend: site.baseurl }})

4. Abrirá a tela de encerramento.
![Janela encerramento]({{ "/assets/img/coleta/janela-encerramento.png" | prepend: site.baseurl }}){:width="700px"}

5. Selecione um dos tipos de encerramento.
![Tipos agendamento]({{ "/assets/img/coleta/tipos-encerramento.png" | prepend: site.baseurl }})

- **Evento:** Ocorrências que indicam que algo inesperado aconteceu e eventualmente será feita uma nova tentativa de contatar esse número.
- **Encerramento:** Ocorrências que invalidam o número, não ocorrerá outra tentativa de contato com o número exceto se for feito uma [volta de status](/fastQuestAdmin/campo/volta-status). 
 
{:start="6"}
6. Selecione a ocorrência. *As ocorrências listadas podem variar de acordo com o que foi selecionado previamente e o que foi cadastrado para o Job no módulo Admin na [tela de Status](/fastQuestAdmin/cadastros/status/)*
![Status de Evento]({{ "/assets/img/coleta/status-evento.png" | prepend: site.baseurl }})

7. Preencha alguma observação para a ocorrência.
![Observação Encerramento]({{ "/assets/img/coleta/observacao-encerramento.png" | prepend: site.baseurl }})

8. Clique em "Salvar".
![Botão Salvar]({{ "/assets/img/coleta/botao-salvar-encerramento.png" | prepend: site.baseurl }})

9. Escolha se deseja "Salvar" ou "Salvar com rediscagem". Ao "Salvar com Rediscagem" você poderá alterar o telefone do cliente e imediatamente discar para o número novo. *A rediscagem só estará disponível caso a ocorrência selecionada não invalide o cliente*.
![Botão Salvar Opções]({{ "/assets/img/coleta/botao-salvar-opcoes-encerramento.png" | prepend: site.baseurl }})

10. Após isto o contato estará encerrado.