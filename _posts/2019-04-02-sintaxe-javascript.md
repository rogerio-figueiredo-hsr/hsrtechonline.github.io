---
layout: post
title:  "Sintaxe Javascript"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/funcoesv2/sintaxeJavascript
pasta: "funcoesv2"
---

# Sintaxe Javascript

# Variáveis
*Variáveis JavaScript são contêineres para armazenar valores de dados.*

No exemplo abaixo x, y e z são variáveis. x recebe 5, y recebe 6 e z recebe a soma de x e y.  
<pre>
<code>var x = 5;
var y = 6;
var z = x + y;
Resultado:  z = 11</code>
</pre>

**Operadores Aritméticos**
<table class="w3-table-all notranslate">
<tbody>
  <tr>
    <th style="width:25%">Operador</th>
    <th>Descrição</th>
    <th>Exemplo</th>
  </tr>
  <tr>
    <td>+</td>
    <td>Adição</td>
    <td>var a = x + y</td>
  </tr>
  <tr>
    <td>-</td>
    <td>Subtração</td>
    <td>var a = x - y</td>
  </tr>
  <tr>
    <td>*</td>
    <td>Multiplicação</td>
    <td>var a = x * y</td>
  </tr>
  <tr>
    <td>/</td>
    <td>Divisão</td>
    <td>var a = x / y</td>
  </tr>
  <tr>
    <td>++</td>
    <td>Incremento</td>
    <td>var a = x++ (atribui x + 1 para a)</td>
  </tr>
  <tr>
    <td>--</td>
    <td>Decremento</td>
    <td>var a = x++ (atribui x - 1 para a)</td>
  </tr>
</tbody></table>

**Operadores de Atribuição**
<table class="w3-table-all notranslate">
  <tbody><tr>
    <th style="width:25%">Operador</th>
    <th>Exemplo</th>
    <th>O mesmo que</th>
  </tr>
  <tr>
    <td>=</td>
    <td>x = y</td>
    <td>x = y</td>
  </tr>
  <tr>
    <td>+=</td>
    <td>x += y</td>
    <td>x = x + y</td>
  </tr>
  <tr>
    <td>-=</td>
    <td>x -= y</td>
    <td>x = x - y</td>
  </tr>
  <tr>
    <td>*=</td>
    <td>x *= y</td>
    <td>x = x * y</td>
  </tr>
  <tr>
    <td>/=</td>
    <td>x /= y</td>
    <td>x = x / y</td>
  </tr>
</tbody></table>  

**Operadores de Comparação**
<table class="w3-table-all notranslate">
  <tbody><tr>
    <th style="width:12%">Operador</th>
    <th>Descrição</th>
    <th>Exemplo</th>
    </tr>
    <tr>
      <td>==</td>
      <td>Igual a</td>
      <td>a == b (Retorna verdadeiro se forem iguais)</td>
    </tr>
    <tr>
      <td>===</td>
      <td>Igual a valor e igual ao tipo (texto/número)</td>
      <td>a === b (Retorna verdadeiro se forem iguais no valor e no tipo (texto com texto, número com número)</td>
    </tr>
    <tr>
      <td>!=</td>
      <td>Diferente</td>
      <td>a != b (Retorna verdadeiro se forem diferentes)</td>
    </tr>
    <tr>
      <td>&gt;</td>
      <td>Maior que</td>
      <td>a > b (Retorna verdadeiro se a for maior que b)</td>
    </tr>
    <tr>
      <td>&lt;</td>
      <td>Menor que</td>
      <td>a < b (Retorna verdadeiro se a for menor que b)</td>
    </tr>
    <tr>
      <td>&gt;=</td>
      <td>Maior que ou igual a</td>
      <td>a >= b (Retorna verdadeiro se a for maior ou igual a b)</td>
    </tr>
    <tr>
      <td>&lt;=</td>
      <td>Menor que ou igual a</td>
      <td>a <= b (Retorna verdadeiro se forem a for menor ou igual a b)</td>
    </tr>
  </tbody>
</table>

**Operadores Lógicos**
<table class="w3-table-all notranslate">
  <tbody>
    <tr>
      <th style="width:12%">Operador</th>
      <th>Descrição</th>
      <th>Exemplo</th>
    </tr>
    <tr>
      <td>&amp;&amp;</td>
      <td>Operador lógico E</td>
      <td>a && b (Retorna verdadeiro se a comparação "ambos" forem iguais ou retornarem verdadeiro e etc.)</td>
    </tr>
    <tr>
      <td>||</td>
      <td>Operador lógico OU</td>
      <td>a || b (Retorna verdadeiro se "um deles" atender a uma determinada condição)</td>
    </tr>
    <tr>
      <td>!</td>
      <td>Operador lógico (Não/Negação)</td>
      <td>!a (Inverte a condição de a. Se originalmente for verdadeiro, inverte para falso)</td>
    </tr>
  </tbody>
</table>

# if/else
*Avalia uma condição no if e executa alguma função caso atenda, senão (else) executa outra função*

<pre>
<code>var opcoesSel = RM("nrquestao").Selecionadas().Contar() 
if (opcoesSel < 5) {
  "Executa qualquer expressão"
}else{
  "Executa outra expressão"
}</code>
</pre>

# for
*Executa o mesmo código repetidas vezes, sempre com um valor diferente.*

<pre>
<code>var opcoes = RM("Q1").Selecionadas().Contar()
for (var i = 1; i <= opcoes; i++) { 
  RM("Q2").Todas().Selecionar(i)
}</code>
</pre>

# switch
*A instrução switch é usada para executar ações diferentes com base em condições diferentes.*

<pre>
<code>switch(expressao) { <b>(Avalia a expressao)</b>
  case x: <b>Caso seja x</b>
    // "Bloco de código para ser executado"
    break;
  case y: <b>Caso seja x</b>
    // "Bloco de código para ser executado"
    break;
  default:<b>Opcional. Caso não seja nenhum dos dois anteriores</b>
    // "Bloco de código para ser executado"
}
