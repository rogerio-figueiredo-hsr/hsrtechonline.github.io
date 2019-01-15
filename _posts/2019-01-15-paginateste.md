---
layout: default
title: "Página Testes"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/teste
pasta: Projetos
teste: [1, 2, 3, 4]
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
    {{ "texto" | append: "teste"}}
    {{ -10 | abs }}
    {{ "texto" | capitalize}}
    {{ page.title | upcase}}
{% endif %}

{% if page.teste == "testando" %}
    {{ page.title | size }}
{% else %}
    {{ page.url }}
    {{ teste }}
{% endif %}

{:start="4"}

1. eqopiewqq
2. qwopeioqweo
3. qwopeiqoe