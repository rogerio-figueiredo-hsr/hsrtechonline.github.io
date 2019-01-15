---
layout: default
title: "Página Testes"
projeto: "fastQuestAdmin"
permalink: /fastQuestAdmin/teste
pasta: Projetos
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
{% endif %}

{:start="4"}

1. eqopiewqq
2. qwopeioqweo
3. qwopeiqoe

<ul>
{% for member in site.data.members %}
  <li>
    <a href="https://github.com/{{ member.github }}">
      {{ member.name }}
    </a>
  </li>
{% endfor %}
</ul>