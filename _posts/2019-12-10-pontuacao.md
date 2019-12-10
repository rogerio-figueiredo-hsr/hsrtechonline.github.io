# Obter Soma Pontuação
*Retorna a soma da pontuação para uma ou mais questões.*

- Sintaxe:
  - `Pontuacao().ObterSomaPontuacao([NRQUESTAOSEQUENCIA])`
- Parâmetros:
  - NRQUESTAOSEQUENCIA: Código das questões entre aspas duplas separadas por vírgula ou variável
- Exemplo 1:
  - `Pontuacao().ObterSomaPontuacao(["Q1","Q2"])`
- Exemplo 2:
  - <pre>
    <code>var nrquestao = (pode ser o retorno de uma função ou estático)
    Pontuacao().ObterSomaPontuacao(nrquestao)</code>
    </pre>
- Resultado:
  - Retorna o valor da soma da pontuação atribuido à(s) questão(ões) declarada(s)
