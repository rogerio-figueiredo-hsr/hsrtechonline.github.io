---
layout: default
title: "Página Testes"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/teste
pasta: Projetos
---

# Testand a página
1. asdaskodd
2. sakkosdapkod
3. askdpoakodsa

- Teste
    **testando**

----
{% assign array = 4, 2, 1, 3 %}

{% assign cont = 0 %}

{% if page.title == "Página Teste" %}
    teste
{% else %}
    {{ "texto" | append: "teste"}}
    {{ -10 | abs }}
    {{ "texto" | capitalize}}
    {{ page.title | upcase}}
{% endif %}

{% if page.teste == "testando" %}
    {{ page.title | size }}
{% else %}
    {{ page.url }}
{% endif %}

{% for cont in (cont...10) %}
    {% increment cont %}
{% endfor %}

{:start="4"}

1. eqopiewqq
2. qwopeioqweo
3. qwopeiqoe