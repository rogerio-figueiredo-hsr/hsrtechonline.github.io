---
layout: post
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

{% assign testarray = "1, 2, 3, 4" | split: ", " %}

{% for i in testarray %}
    {{i}}
{% endfor %}

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

{% assign nome = "Asaopdsdasjd" %}

{% if nome.size > 10 %}
    {{ nome }}, ok
{% else %}
    {{ nome }}, not ok
{% endif %}

1. eqopiewqq
2. qwopeioqweo
3. qwopeiqoe