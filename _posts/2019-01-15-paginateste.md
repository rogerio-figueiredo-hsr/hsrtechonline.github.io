---
layout: default
title: "Página Testes"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/teste
pasta: Projetos
teste: "testando"
---

# Testando a página
1. asdaskodd
2. sakkosdapkod
3. askdpoakodsa

- Teste
    **testando**

----

{% if page.title == "Página Teste" %}
    teste
{% else %}
    <h1>{{ "texto" | append: "teste"}}</h1>
    <h1>{{ -10 | abs }}</h1>
    <h1>{{ "texto" | capitalize}}</h1>
    <h1>{{ page.title | upcase}}</h1>
{% endif %}

{% if page.teste == "testando"}
    {{ page.title | size }}
{% else %}
    <p>{{ page.url }}</p>

{:start="4"}

4. eqopiewqq
5. qwopeioqweo
6. qwopeiqoe